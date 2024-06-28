## 目次

- [目次](#目次)
- [Next.JSプロジェクトの作成](#nextjsプロジェクトの作成)
  - [最新バージョン](#最新バージョン)
  - [特定のバージョンを指定して作成する](#特定のバージョンを指定して作成する)
- [Gitの`.gitignore`ファイルを簡単に作成する](#gitのgitignoreファイルを簡単に作成する)
  - [方法1: GitHubの.gitignoreテンプレートを利用する](#方法1-githubのgitignoreテンプレートを利用する)
  - [方法2: コマンドラインツールを利用する](#方法2-コマンドラインツールを利用する)

## Next.JSプロジェクトの作成

### 最新バージョン
以下のコマンドで最新バージョンのNext.JSを使用したプロジェクトが作成される
```
npx create-next-app nextjs-project --typescript --eslint --use-npm
cd nextjs-project
```

### 特定のバージョンを指定して作成する

バージョンを指定するには、`npm i`にてプロジェクトで使用したいNext.JSのバージョンを明示する  
以下のコマンドは `12.3.4`のバージョン指定でプロジェクトを作成
```
npx create-next-app@12.3.4 nextjs-project-12-3-4 --typescript --eslint --use-npm
cd nextjs-project-12-3-4
npm i next@12.3.4
```



## Gitの`.gitignore`ファイルを簡単に作成する

### 方法1: GitHubの.gitignoreテンプレートを利用する  
[GitHubの.gitignoreテンプレート](https://github.com/github/gitignore)にアクセス  
プロジェクトに合ったテンプレートを選び、その内容をコピー  
プロジェクトのルートディレクトリに`.gitignore`ファイルを作成し、コピーした内容を貼り付ける  

### 方法2: コマンドラインツールを利用する  
`gitignore.io`(https://www.toptal.com/developers/gitignore/)というサービスを利用して、簡単にカスタム`.gitignore`ファイルを生成できる  

コマンドラインで以下のコマンドを実行（例として、Node.jsとReactとNodeとASP.NETとそれぞれのOS環境のプロジェクト用の`.gitignore`を生成する場合）:
```
curl -L -s https://www.toptal.com/developers/gitignore/api/nextjs,react,macos,windows,linux,node,aspnetcore > .gitignore
```

このコマンドは`node`と`react`と`Node`と`ASP.NET`とそれぞれの`OS環境`に適した`.gitignore`ファイルを生成してくれます。