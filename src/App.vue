<template>
  <my-tree :tree-data="treeData" @node-click="nodeClick"></my-tree>
</template>

<script>
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
import myTree from '@/components/myTree.vue'
export default {
  components: {
    myTree
  },
  data() {
    return {
      treeData: treeData
    }
  },
  methods: {
    nodeClick(val) {
      console.log(val)
    }
  }
}
</script>
