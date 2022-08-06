# github
## gtihub actions
### steps

### reference
 - [official](https://docs.github.com/ja/)
 - [やってみる](https://iwb.jp/automatically-run-linter-push-github-actions/)

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