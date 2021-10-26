# iamui

### 打包 iamui

确保安装了 node、npm、npx。

在项目根目录使用 npm 初始化
```
npm init
```

安装 postcss 和 postcss-impor 插件
```
npm i postcss-cli@6.1.3 -D

npm i postcss-import@12.0.1 -D
```

将内容集中到一个 css 文件中
```
npx postcss src/iamui-ui.css -o dist/iamui-ui.css -u postcss-import --no-map
```

安装插件 cssnano
```
npm i cssnano@4.1.10 -D
```

压缩
```
npx postcss src/iamui-ui.css -o dist/iamui-ui.min.css -u postcss-import cssnano --no-map
```