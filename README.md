# angular-show-more
AngularJS directive that limit text and adds show more / show less links to your text when it exeeds certain limit of characters. Only angularjs is required.

##jsfiddle demo

[Codepen demo](http://jsfiddle.net/janakbhatta/0p6j9ghk/ "JsFiddle: AngularJS Show More Directive")


## Install client side
```bash
$ bower install angular-read-more --save-dev 
```

## Run example locally
```bash
$ git clone
$ npm install
$ bower install
$ gulp watch
```

## Test locally
```bash
$ git clone
$ npm install
$ bower install
$ gulp karma
```

## How to use in HTML
Include JS script
```html
<script src="/bower_components/angular-read-more/readmore.min.js"></script>
```

As element
```html
<hm-read-more
		hm-text="{{ text }}" 
		hm-limit="100" 
		hm-more-text="read more" 
		hm-less-text="read less"
		hm-dots-class="dots"
        hm-link-class="links">
</hm-read-more>
```

As attribute
```html
<div hm-read-more
		hm-text="{{ text }}" 
		hm-limit="100" 
		hm-more-text="read more" 
		hm-less-text="read less"
		hm-dots-class="dots"
        hm-link-class="links">
</div>
```

* `hm-text` - full text
* `hm-limit` - number > 0 of maximum characters before adding "..." and the more/less text. Default: unlimited
* `hm-more-text` - link text for read more. Default: Read more
* `hm-less-text` - link text for read less. Default: Read less
* `hm-dots-class` - css class for dots
* `hm-link-class` - css class for links of read more/read less text

##License
angular-read-more is licensed under the MIT license.

##Release new Github and Bower version
```bash
gulp bump
gulp build
git add .
git commit -m ""
git push
```
Use Github UI to create new tag and release
```bash
bower register angular-read-more git://github.com/ismarslomic/angular-read-more.git
```
