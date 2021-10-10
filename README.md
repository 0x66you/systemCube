<h2 align="center">
  🔖 Minimalist design essay template 📎 <a href="https://0x66you.github.io/system_cube/">system_cube</a>&nbsp;(Live demo)
</h2>

<p align="center"><img src="https://i.postimg.cc/WpJVCQKQ/LIST-UM-2.png" width="860" alt="workerize"></p>

## About project

version | detail and fixes
:------------: | :-------------:
v0.5  | load error with 'Next' 'Prev'
v1.5  | 'Next' jumps to 2nd page<br>when on home page
### v0.5 fix
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

## License

[MIT License](https://oss.ninja/mit/0x66you) © Yeh,Chun-Chen
