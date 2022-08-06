# github
This repository is the memo related to git.

---
## gtihub actions
### steps
1. [GitHub Actionsでpushした際に自動的にLinterを実行する方法](https://iwb.jp/automatically-run-linter-push-github-actions/)
2. [Node.js のビルドとテスト](https://docs.github.com/ja/actions/automating-builds-and-tests/building-and-testing-nodejs)

### reference
 - [official](https://docs.github.com/ja/)
 - [Github Actions のビルドマトリックスを使う](https://ema-hiro.hatenablog.com/entry/2020/12/15/123210)
 - [if-present](https://manpages.ubuntu.com/manpages/impish/man1/npm-run-script.1.html)

---
## ES Lint
### steps
1. install
   ``` shell
    npm init @eslint/config
      ✔ How would you like to use ESLint? · problems
      ✔ What type of modules does your project use? · esm
      ✔ Which framework does your project use? · None
      ✔ Does your project use TypeScript? · Yes
      ✔ Where does your code run? · browser, node
      ✔ What format do you want your config file to be in? · YAML
      ✔ Would you like to install them now? · Yes
      ✔ Which package manager do you want to use? · npm
   ```
2. set npm command
   ``` json
    "scripts": {
      "lint": "eslint *.ts*"
    },
   ```
3. install air-bnb config & add extends to config
   ```shell
    # reactを利用しない場合
    npm i -D eslint-config-airbnb-base eslint-plugin-import
   ```
   ```yml
    extends:
      - airbnb-base  # reactを利用しない場合
   ```
4. npm run lint
   3.でconfig(ルール)を設定しないとエラーを出力しない。
### reference
 - [official](https://eslint.org/docs/latest/user-guide/getting-started)
 - [eslint-config-airbnb](https://qiita.com/sugx2/items/ed58605e4e12519876fd)
 - [Node.js & TypeScriptのプロジェクト作成](https://typescript-jp.gitbook.io/deep-dive/nodejs)