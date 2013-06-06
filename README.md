sham-spinner
===========

###About
Mixins for scalable and color-able — is that a word? — spinners.

These spinners use inline SVG so there are no images! They look great at any size, on any screen. There's virtually no loading time, so you don't need a spinner while your spinner loads... ;)

This repo features several commonly used spinner styles — pinwheel, dots, circular, peacock, and the ever-ubiquitous spokes — but feel free to add more with pull requests. Since we're using mixins, we don't have to worry to much about bloat.

By passing in $size and $color variables, spinners are easily customized and reuseable throughtout your project.


###Installation
Naturally, you'll need SASS (http://sass-lang.com) to use these mixins.

Install using Bower (http://bower.io)

    bower install simple-spinner

OR simply include the main SCSS file early in your stylesheets directory.

In your project, add markup and styles along these lines:

    <div class="sham-spinner-circular"></div>

    .my-awesome-circular-spinner {
      @include sham-spinner-circular(red, 32px);
      // optional stuff to define the container
      width               : 42px;
      height              : 42px;
    }

Include any color and size that pleases you. Just make sure your container is large enough properly contain the background image.

SVG is supported in most browsers. You'll need set up a fallback for older IE8 and older browsers.


###About Sham
We here at Identified.com use automative-themed names for our repos.

"Sham" – derived from chamois, a cloth comonly used to polish cars — is our all-purpose toolbox containing SASS mixins and variables to help us quickly build web apps. Add these classes in your markup or use @extend .className in your CSS to use.
