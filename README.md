# holo-ui

## 项目说明
### 1.在哪里写组件
  组件统一放置在packages目录下。<br />
  单个组件以文件夹存放，例如新加一个button组件，则新建一个button文件夹

  :::  warning Note
  .<br />
  ├── button _(**实例展示**)_<br />
  │   ├── `button.vue` _(**组件**)_<br />
  │   └── `index.ts` _(**输出，命名只能使用index.ts,写法可参考demo**)_<br />
  :::

### 2.文档在哪里写
  文档统一在docs里面编写，这一块的内容我也还在学习，暂时不晓得写啥，先放着
  文档里面可以直接调用组件，所以，是否要单独写组件，后面再来看，反正example 已经准备好了

## 目录结构

<!-- textlint-disable terminology -->
::: warning Note
.<br />
├── docs _(**文档编写**)_<br />
│   ├── .vuepress _(**存放vurpress全局的配置、组件、静态资源等**)_<br />
│   │   ├── `config.js` _(**配置文件的入口文件**)_<br />
│   │ <br />
│   └── README.md _(**文档首页**)<br />
│ <br />
├── example _(**实例展示**)_<br />
│   ├── assets _(**静态资源**)_<br />
│   ├── router _(**路由配置**)_<br />
│   ├── views _(**存放页面**)_<br />
│   ├── `app.vue` _(**layout页面**)_<br />
│   └── `main.ts` _(**入口文件**)_<br />
├── packages _(**存放组件**)_<br />
│   └── `index.ts` _(**入口文件**)_<br />
└── package.json<br />
:::
<!-- textlint-enable -->

## 开发说明

### 如何运行项目
运行 npm run serve          以开发模式跑 example 目录<br />
运行 npm run docs:dev       以开发模式跑 文档<br />
运行 npm run build          打包packages目录，生成组件库，组件库生成在lib目录下<br />
