# Background Animation

Simple background color animation with keyframes

**Still in beta**  

#### Live Demo :

Example : http://codepen.io/Tonours/pen/Ehfxd


## How it works
### SCSS
    @import "mixins";
        
    // Colors list
    $colors: #69D2E7, #A7DBD8, #E0E4CC, #F38630, #FA6900;
    
    // Enable mixin
    // How to use : 
    // @include background-animation($name, $colors, $container, $duration, $timing, $iteration, $direction);
    @include background-animation('bgcolor', $colors, 'body', '20s', 'ease-in', 'infinite', 'alternate');


### CSS
    <!-- Generated code -->
    @-webkit-keyframes bgcolor {
      0% {
        background: #69d2e7; }

      25% {
        background: #a7dbd8; }

      50% {
        background: #e0e4cc; }

      75% {
        background: #f38630; }

      100% {
        background: #fa6900; } 
      }

    @keyframes bgcolor {
      0% {
        background: #69d2e7; }

      25% {
        background: #a7dbd8; }

      50% {
        background: #e0e4cc; }

      75% {
        background: #f38630; }

      100% {
        background: #fa6900; } 
      }

    body {
      animation-name: bgcolor;
      animation-duration: 20s;
      -webkit-animation-name: bgcolor;
      -webkit-animation-duration: 20s;
      animation-iteration-count: infinite;
      -webkit-animation-iteration-count: infinite;
      animation-direction: alternate;
      -webkit-animation-direction: alternate;
      animation-timing-function: ease-in;
      -webkit-animation-timing-function: ease-in;
      -webkit-animation-fill-mode: backwards;
      animation-fill-mode: backwards; }

## How to launch Application ? 

```
  gem install middleman
  git clone https://github.com/Tonours/background-transition.git
  cd background-animation.git
  bundle install
  middleman server
```



