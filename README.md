# component-recurse-demo
使用Vue组件递归，实现树形结构数据的渲染

掘金地址：https://juejin.cn/post/7056922161788747789

```
// 树形结构数据：
const treeData = [
  { id: 1, name: '一级1' },
  {
    id: 2,
    name: '一级2',
    children: [
      { id: 3, name: '二级2-1' },
      { id: 4, name: '二级2-2' }
    ]
  },
  {
    id: 5,
    name: '一级3',
    children: [
      {
        id: 6,
        name: '二级3-1',
        children: [
          { id: 7, name: '三级3-1-1' },
          { id: 8, name: '三级3-1-2' }
        ]
      },
      { id: 9, name: '二级3-2' },
      { id: 10, name: '二级3-3' }
    ]
  }
]
```

## Project setup

```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
