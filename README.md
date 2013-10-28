# Background Transition

Simple background color animation with keyframes

**Still in beta**  


## How it's work
### SCSS
    @import "mixins";
        
    // Colors list
    $colors: #69D2E7, #A7DBD8, #E0E4CC, #F38630, #FA6900;
    
    // Enable mixin
    // How use : 
    // @include background-transition($name, $colors, $container, $duration, $timing, $iteration, $duration);
    @include background-transition('bgcolor', $colors, 'body', '20s', 'ease-in', 'infinite', 'alternate');

### CSS
    <!-- Generated code -->
    @-webkit-keyframes bgcolor {
    0% {
      background: #69d2e7; }

    20% {
      background: #69d2e7; }

    40% {
      background: #a7dbd8; }

    60% {
      background: #e0e4cc; }

    80% {
      background: #f38630; }

    100% {
      background: #fa6900; }
    }
    @keyframes bgcolor {
      0% {
        background: #69d2e7; }

      20% {
        background: #69d2e7; }

      40% {
        background: #a7dbd8; }

      60% {
        background: #e0e4cc; }

      80% {
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

## How launch Application ? 

```
  gem install middleman
  git clone https://github.com/Tonours/background-transition.git
  cd background-transition.git
  bundle install
  middleman server
```



