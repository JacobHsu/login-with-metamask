# login-with-metamask

[One-click Login with Blockchain: A MetaMask Tutorial](https://www.toptal.com/ethereum/one-click-login-flows-a-metamask-tutorial)  
amaurymartiny/[login-with-metamask-demo](https://github.com/amaurymartiny/login-with-metamask-demo)  

## MetaMask

[To develop for MetaMask](https://metamask.github.io/metamask-docs/Main_Concepts/Getting_Started)  
[No Longer Injecting web3.js](https://medium.com/metamask/no-longer-injecting-web3-js-4a899ad6e59e)

## Docs

[lerna](https://lerna.js.org/)  
[Docker Hub](https://hub.docker.com/)  
[Get started with Docker Compose](https://docs.docker.com/compose/gettingstarted/#step-8-experiment-with-some-other-commands)

## lerna

`lerna init`

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