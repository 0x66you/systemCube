<h2 align="center">
  🔖 Minimalist design essay template 📎 <a href="https://0x66you.github.io/system_cube/">system_cube</a>&nbsp;(Live demo)
</h2>

<p align="center"><img src="https://i.postimg.cc/WpJVCQKQ/LIST-UM-2.png" width="860" alt="workerize"></p>

## About project
Essays are written in external files, **asynchronously loaded in when called**.<br>
Random text generated with [Lorem Ipsum](https://www.lipsum.com).
```js
setPageContent(...){
    ...
    $.ajax(
        {
            ...
            success: function(data){
                console.log(`[success] loaded ${instance_id}..`);
                $(`#${instance_id}`).load(external_url);
            },
            error: function(xhr){
                console.log(`[failed] unable to load essay1{xhr.status}`)
            }
        }
    );
}
```
Homepage will **NOT** be shown again after switching to other pages,<br>
refreshing the page brings you back to homepage.<br>
Feel free to download and customize to your liking.

version | detail | solved
:------------: | :-------------: | :-------------:
v0.5  | 'Next' 'Prev' load error  | ✅
v1.5  | 'Next' jumps to 2nd page<br>if clicked on home page | ❌
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
## Prerequisites
* Html Css (duh!)
* jquery ajax
* bootstrap v4.1
* vue.js

## License

[MIT License](https://oss.ninja/mit/0x66you) © Yeh,Chun-Chen
