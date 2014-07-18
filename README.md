## Install

*Requirements*

Node / NPM

Bower (Package Manager)

```
npm install bower -g
```

Inside your project run:

```
bower install x-tag-slidebox
```

This downloads the component and dependencies to ./components




## Syntax

Slidebox allows you to create slides of any content and then transition between them.  It supports x and y axis transitions.

```
<x-slidebox>
  <x-slides>
    <x-slide><img src="demo/birnimal-calendar.png" /></x-slide>
    <x-slide><img src="demo/birnimal-graph.png" /></x-slide>
    <x-slide><img src="demo/birnimal-detail.png" /></x-slide>
    <x-slide><img src="demo/birnimal-settings.png" /></x-slide>
  </x-slides>
</x-slidebox>
```


## Events
```slideend``` is fired at the end of each transition.

```
  document.getElementsByTagName('x-slidebox')[0].addEventListener('slideend', function(e){
    
  });

```

## Usage

```
  var slidebox = document.getElementsByTagName('x-slidebox')[0];
  slidebox.slideNext();
  slidebox.slidePrevious();
  slidebox.slideTo(1); // index of desired x-slide
  
  slidebox.orientation = 'y';  // slide veritically 

```


