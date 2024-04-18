jiacrontab-frontend 前端代码
### 后端地址 https://github.com/topascend/jiacrontab
## 安装包管理工具
[安装yarn](https://yarnpkg.com)
```
npm install -g yarn
```
## 安装依赖

```
yarn
yarn add react-scripts-ts --dev
```

## 配置代理

修改 package.json 代理使接口指向 jiacrontab 服务

```json
"proxy": {
        "/v1": {
            "target": "http://localhost:20000",
            "changeOrigin": true
        },
        "/v2": {
            "target": "http://localhost:20000",
            "changeOrigin": true
        }
    }
```

## 开发环境运行

```
yarn start
```

## 生产环境编译

```
yarn build
```

## 打包jiacrontab
```sh
生产环境编译后直接将 build的全部内容复制到后端 jiacrontab/jiacrontab_admin/assets
```
