# Vanilla-JS - CODES

## .ready

``` js
```
 Jquery  
``` js
$('document').ready(function(){

}};
```
 Vanilla JS
``` js
document.addEventListener('DOMContentLoaded', function(){

});
```

## .offset
jquery
``` js

```

Vanilla JS
``` js

```


<!-- teste -->

//Functions 
function offset(elt) {
var rect = elt.getBoundingClientRect(), bodyElt = document.body;

return {
  top: rect.top + bodyElt .scrollTop,
  left: rect.left + bodyElt .scrollLeft
}
}


document.addEventListener('DOMContentLoaded', function(){

//elementos
var toggle = document.getElementsByClassName('toggle');
		nav    = document.getElementById('nav');
		logo   = document.getElementById('logo');

//clicar no toggle
for(var z =0; z < toggle.length; z++){
    var elem = toggle[z];   
    elem.onclick = function(){        
    	elem.classList.toggle('toggle-ativo');
    	nav.classList.toggle('nav-ativo');
    };
}

window.addEventListener('scroll', function() {
	// var offsetLogo = offset(logo);
	// 		logoHeight = offsetLogo.top + logo.offsetHeight;
		var	offsetWindow = window.pageYOffset;

			if (offsetWindow >= 45 ) {
				logo.classList.add('logo-scroll');
			} else {
				logo.classList.remove('logo-scroll');
			}

	// console.log(offsetWindow);

});


});
