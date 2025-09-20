プロフィールをGitHub Pagesで公開しています

https://yowatanabe.github.io/




GitHubリポジトリを作成
リポジトリ名はusername.github.io

作成したリポジトリをローカルにクローン



Hugoをインストールする
brew install hugo



サイトを作成

hugo new site yowatanabe.github.io

```
$ hugo new site yowatanabe.github.io
Congratulations! Your new Hugo site was created in /Users/bfl/src/portfolio/yowatanabe.github.io.

Just a few more steps...

1. Change the current directory to /Users/bfl/src/portfolio/yowatanabe.github.io.
2. Create or install a theme:
   - Create a new theme with the command "hugo new theme <THEMENAME>"
   - Or, install a theme from https://themes.gohugo.io/
3. Edit hugo.toml, setting the "theme" property to the theme name.
4. Create new content with the command "hugo new content <SECTIONNAME>/<FILENAME>.<FORMAT>".
5. Start the embedded web server with the command "hugo server --buildDrafts".

See documentation at https://gohugo.io/.
 ~/src/portfolio  $ 
$
```

```
$ tree
.
├── archetypes
│   └── default.md
├── assets
├── content
├── data
├── hugo.toml
├── i18n
├── layouts
├── static
└── themes

9 directories, 2 files
```

テーマを追加

https://themes.gohugo.io/themes/hugo-theme-hello-friend-ng/


```
git submodule add --depth=1 https://github.com/rhazdon/hugo-theme-hello-friend-ng.git themes/hugo-theme-hello-friend-ng
echo "theme = 'hugo-theme-hello-friend-ng'" >> hugo.toml
```

もしテーマを削除したい場合

```
# 1. サブモジュールを deinit して無効化
git submodule deinit -f themes/hugo-theme-hello-friend-ng

# 2. サブモジュールを Git 管理から削除
git rm -f themes/hugo-theme-hello-friend-ng

# 3. キャッシュを削除 (.git/modules 以下に残るデータ)
rm -rf .git/modules/themes/hugo-theme-hello-friend-ng
```




```
git init
git remote add origin git@github.com:yowatanabe/yowatanabe.github.io.git
git push -u origin main
```
