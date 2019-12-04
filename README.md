# login-with-metamask

[One-click Login with Blockchain: A MetaMask Tutorial](https://www.toptal.com/ethereum/one-click-login-flows-a-metamask-tutorial)  
amaurymartiny/[login-with-metamask-demo](https://github.com/amaurymartiny/login-with-metamask-demo)  

## Start the demo using Yarn:

From the root folder of this repo, run

```bash
yarn install # Install the dependencies
yarn start # Will launch the frontend and the backend at the same time
```

The backend should be running on `localhost:8000`, and the frontend on `localhost:3000`.

Alternatively, you can start the frontend and the backend separately:

```bash
# Start the backend
cd packages/backend
yarn start

# Start the frontend
cd packages/frontend
yarn start
```

## Tests

Since this project is a demo, I haven't written any tests for it. Only code linting is performed, via prettier, which you can run using `yarn lint`.

## MetaMask

[To develop for MetaMask](https://metamask.github.io/metamask-docs/Main_Concepts/Getting_Started)  
[No Longer Injecting web3.js](https://medium.com/metamask/no-longer-injecting-web3-js-4a899ad6e59e)

## Docs

[lerna](https://lerna.js.org/)  
[Docker Hub](https://hub.docker.com/)  
[Get started with Docker Compose](https://docs.docker.com/compose/gettingstarted/#step-8-experiment-with-some-other-commands)

## lerna

`lerna init`

```js
// 并行执行所有packages的start命令
$ lerna run start --parallel
```

[基于lerna+yarn workspaces的monorepo项目实践](https://juejin.im/post/5c94fdccf265da60fc46a48f)

## npm 

[![NPM](https://nodei.co/npm/@types/jest.png?downloads=true&stars=true)](https://nodei.co/npm/@types/jest/)
`npm install --save-dev @types/jest`
[![NPM](https://nodei.co/npm/prettier.png?downloads=true&stars=true)](https://nodei.co/npm/prettier/)
`npm i prettier --save-dev`
[Configuration File](https://prettier.io/docs/en/configuration.html)

[![NPM](https://nodei.co/npm/typescript.png?downloads=true&stars=true)](https://nodei.co/npm/typescript/)
`npm i typescript --save-dev`
[tsconfig.json](https://www.tslang.cn/docs/handbook/tsconfig-json.html)

### frontend

[![NPM](https://nodei.co/npm/react-blockies.png?downloads=true&stars=true)](https://nodei.co/npm/react-blockies/)
[![NPM](https://nodei.co/npm/web3.png?downloads=true&stars=true)](https://nodei.co/npm/web3)
[![NPM](https://nodei.co/npm/jwt-decode.png?downloads=true&stars=true)](https://nodei.co/npm/jwt-decode)

### backend

[![NPM](https://nodei.co/npm/nodemon.png?downloads=true&stars=true)](https://nodei.co/npm/nodemon/)
nodemon 用來監察檔案的改變，重新觸發
[![NPM](https://nodei.co/npm/ts-node.png?downloads=true&stars=true)](https://nodei.co/npm/ts-node/)
`ts-node` 通過 `tsconfig.json` 的設定，對 `index.ts` 進行自動編譯成為 js


[![NPM](https://nodei.co/npm/sequelize.png?downloads=true&stars=true)](https://nodei.co/npm/sequelize/)
[使用Sequelize](https://www.liaoxuefeng.com/wiki/1022910821149312/1101571555324224) 使用 JavaScript 的 ORM (Object-Relational Mapping)
[![NPM](https://nodei.co/npm/sqlite3.png?downloads=true&stars=true)](https://nodei.co/npm/sqlite3/)

[![NPM](https://nodei.co/npm/ethereumjs-util.png?downloads=true&stars=true)](https://nodei.co/npm/ethereumjs-util/)
[![NPM](https://nodei.co/npm/eth-sig-util.png?downloads=true&stars=true)](https://nodei.co/npm/eth-sig-util/)

[Express + JWT用户认证最轻实践](https://juejin.im/post/5b06c6baf265da0db4791805)
[![NPM](https://nodei.co/npm/express.png?downloads=true&stars=true)](https://nodei.co/npm/express/)
[![NPM](https://nodei.co/npm/express-jwt.png?downloads=true&stars=true)](https://nodei.co/npm/express-jwt/)
[![NPM](https://nodei.co/npm/jsonwebtoken.png?downloads=true&stars=true)](https://nodei.co/npm/jsonwebtoken/)

深入理解 TypeScript [@types](https://jkchao.github.io/typescript-book-chinese/typings/types.html)  

## References

[lerna管理前端packages的最佳实践](https://juejin.im/post/5a989fb451882555731b88c2)
[Semver(语义化版本号)](https://juejin.im/post/5ad413ba6fb9a028b5485866)
[web3.js 1.0 API官方文档中文版](http://cw.hubwiz.com/card/c/web3.js-1.0/) 
[Docker Compose 建置 Web service 起步走入門教學](https://blog.techbridge.cc/2018/09/07/docker-compose-tutorial-intro/)
[如何在我的電腦上啟用虛擬化技術](https://support.bluestacks.com/hc/zh-tw/articles/115003174386-如何在我的電腦上啟用虛擬化技術-VT-)

### debug

`frontend> docker run -d -p 3000:3000 login-frontend`  
> C:\Program Files\Docker\Docker\Resources\bin\docker.exe: Error response from daemon: pull access denied for login-frontend, repositoryied for login-frontend, repository does not exist or may require 'docker login': denied: requested access to the resource is denied.

Docker Desktop login

### notes

 Run `npm install -g npm` to update!  version of npm

```bash
docker --version
docker-compose --version
```

查看docker的镜像文件 `docker images` 
启动我们的镜像 `docker run -d -p 8000:8000 login-backend`


找到要刪除的 image 的 image id 後, 便可以執行以下指令刪除:
`docker images`  
`docker rmi image_id`

 