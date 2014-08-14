#### Intro - Get to know the group

* What's your level of CSS experience
* Do you know any programming languages?
* What's the most complex thing you've done with SASS

#### How the meetup will Work

* Each Meetup will be targeted to a specific skill level (Basic/Advanced) ideally with some hands-on time in sassmeister
* The meetup will start with a mini-demo of something at the opposite skill level of main content
* Then we jump into sassmeister.com and do some hands on
* After the meetup we'll grab a pint nearby


####Hands-on

* Breakpoint Intro - http://sassmeister.com/gist/73a53395a4df14a38aab
* no-query support by class - http://sassmeister.com/gist/7b8dded03df82d92970c
* No query support by File - http://sassmeister.com/gist/df87e8fe8e5ba8985201
* Singularity - Setup Mobile First  http://sassmeister.com/gist/47e5f7a46938110fca6f
* Singularity - 960gs http://sassmeister.com/gist/c0f9776f4a0e3fcc9fc8
* Singularity - Non symmetric Grid - http://sassmeister.com/gist/861018f358c9c61ea8d1


------

#### links

* http://www.browsersync.io/
* http://breakpoint-sass.com/
* https://github.com/Team-Sass/Singularity

#### notes

    $breakpoint-no-query-fallbacks

#### no-query-fallback

* https://github.com/Team-Sass/breakpoint/wiki/No-Query-Fallbacks

#### sass placeholder

    %demo--base {
      background-color: rgba(255,100,100, 0.5);
      border: 2px dashed grey;
      text-align: center;
      padding-top: 5em;
      padding-bottom: 5em;
      margin-bottom: 1em;
    }

    header {
      @extend %demo--base;
    }

#### sass mixin

    // Let's make a mixin to help style our demo blocks
    @mixin demo($padding: 5em, $background-color:red ){
      padding-top: $padding;
      padding-bottom: $padding;
      background-color: rgba($background-color, 0.5);
      border: 2px dashed $background-color;
    }

    $background-color:red => :red is the default value, in case you aren't supplied a background-color.

    @include demo() => uses padding 5em, background-color red
    @include demo(10em, white) => uses padding 10em, background-color white

#### singularity notes

will need to use clear: left/right/both; otherwise your grids will push against each other.

https://github.com/Team-Sass/Singularity/wiki/Installation#singularity-demos

**isolation approach**

flexbox => css3/4
