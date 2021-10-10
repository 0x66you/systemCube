<h2 align="center">
  🔖 Minimalist design essay template 📎 <a href="https://0x66you.github.io/system_cube/">system_cube</a>&nbsp;(Live demo)
</h2>

<p align="center"><img src="https://i.postimg.cc/WpJVCQKQ/LIST-UM-2.png" width="860" alt="workerize"></p>

## About project
version | detail and fixes
------------ | -------------
v0.5 before release | load error with Next Prev
Content in the first column | Content in the second column
### v0.5 solved
```js
methods:{
    itemPrevious(){
        ...
        num = this.item;
        this.setPageContent(num,this.catalogue[num-1].url,this.catalogue[num-1].id)
    },
    itemNext(){
        ...
        num = this.item;
        this.setPageContent(num,this.catalogue[num-1].url,this.catalogue[num-1].id)
    }
```
