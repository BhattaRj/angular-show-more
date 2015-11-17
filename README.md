# angular-show-more
AngularJS directive that limit text and adds show more / show less links to your text when it exeeds certain limit of characters. Only angularjs is required.

##Codepen demo

[Codepen demo](http://codepen.io/BhattaRj/pen/GpzPqY?editors=001 "JsFiddle: AngularJS Show More Directive")


## How to use in HTML

As element
```html

<show-more text="book.descripton" limit="170">

```

As attribute
```html

<div show-more text="book.descripton" limit="170"></div>
```

* `text` - full text
* `limit` - number > 0 of maximum characters before adding "..." and the more/less text. Default: unlimited


##License
angular-read-more is licensed under the MIT license.


