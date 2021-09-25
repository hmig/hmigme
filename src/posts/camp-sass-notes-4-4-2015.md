---
layout: layouts/post.njk
title: Camp Sass Notes (4/4/2015)
date: 2015-04-05T03:44:56.085Z
---
[Twitter Tweet](https://platform.twitter.com/embed/Tweet.html?dnt=false&embedId=twitter-widget-1&features=eyJ0ZndfZXhwZXJpbWVudHNfY29va2llX2V4cGlyYXRpb24iOnsiYnVja2V0IjoxMjA5NjAwLCJ2ZXJzaW9uIjpudWxsfSwidGZ3X2hvcml6b25fdHdlZXRfZW1iZWRfOTU1NSI6eyJidWNrZXQiOiJodGUiLCJ2ZXJzaW9uIjpudWxsfSwidGZ3X3NwYWNlX2NhcmQiOnsiYnVja2V0Ijoib2ZmIiwidmVyc2lvbiI6bnVsbH0sInRmd192ZGxfY2hpcnBfMTI3OTQiOnsiYnVja2V0IjoidmRsX29ubHkiLCJ2ZXJzaW9uIjozfX0%3D&frame=false&hideCard=false&hideThread=false&id=584357817689239552&lang=en&origin=https%3A%2F%2Fispeakincode.com%2F&sessionId=2db000740eba09639b54837c8f4cb465dda5e1b5&theme=light&widgetsVersion=1890d59c%3A1627936082797&width=550px)

[Camp Sass](http://campsass.com/2015/) was a blast! Thank you to everyone that made it happen! Here are my notes:

## Micah Godbolt – Visual Regression Testing

So, what is visual regression testing? It’s pixel by pixel comparison (orig, new, diff).

### Variations of visual diffing:

* page based vs component
* comp vs baseline
* headless browser vs desktop browser
* GUI vs command line
* extras – css unit testing, scripting libraries

### Screenshot Comparison Tools:

1. [Wraith](https://github.com/BBC-News/wraith)

* Page based
* comp or baseline
* headless browser
* command line

2. [PhantomCSS](https://github.com/Huddle/PhantomCSS)

* comp based diffing
* baseline
* headless
* command line
* exras – scripting lib

### LINKS

* DEMOS – <https://github.com/micahgodbolt/visual-regression-demo>
* Podcast – <https://www.youtube.com/user/sassbites>

## Bermon Painter – Modular Sass

How do you create scalable websites? Break things down to components!

### 3 methodologies – oocss, smacss, bem

1. [OOCSS](https://github.com/stubbornella/oocss/wiki) – a.k.a. Object Oriented CSS Two main principals, separate:

* structure from skin
* container from content

2. [SMACSS](https://smacss.com/) (scalable and modular architecture for css)

* base (reset, default typography)
* layout (headers footers)
* modules ()
* states (.is-active)
* themes ()

3. [BEM](https://en.bem.info/method/) (block, element, modifier)

* [BEM 101 via css-tricks](https://css-tricks.com/bem-101/)

4. SMABEMOOCSS? JK! 

[Twitter Tweet](https://platform.twitter.com/embed/Tweet.html?dnt=false&embedId=twitter-widget-2&features=eyJ0ZndfZXhwZXJpbWVudHNfY29va2llX2V4cGlyYXRpb24iOnsiYnVja2V0IjoxMjA5NjAwLCJ2ZXJzaW9uIjpudWxsfSwidGZ3X2hvcml6b25fdHdlZXRfZW1iZWRfOTU1NSI6eyJidWNrZXQiOiJodGUiLCJ2ZXJzaW9uIjpudWxsfSwidGZ3X3NwYWNlX2NhcmQiOnsiYnVja2V0Ijoib2ZmIiwidmVyc2lvbiI6bnVsbH0sInRmd192ZGxfY2hpcnBfMTI3OTQiOnsiYnVja2V0IjoidmRsX29ubHkiLCJ2ZXJzaW9uIjozfX0%3D&frame=false&hideCard=false&hideThread=false&id=584419444463632384&lang=en&origin=https%3A%2F%2Fispeakincode.com%2F&sessionId=2db000740eba09639b54837c8f4cb465dda5e1b5&theme=light&widgetsVersion=1890d59c%3A1627936082797&width=550px)

## Una Kravets – Open Source Design

Innovation/Revolution comes about in tech in (usually) one of three ways:

1. government funding

2. big business

3. **open source** 

### GOALS:

1. encourage a more open design/dev workflow

   * positive reinforcement #littlewins
2. foster design participation in the open source community

### CARE Method

#### \[C]ommunication

* label issues properly (design needed, issue)
* use a lot of images

#### \[A]ccessibility

* getting started docs/wikis
* about doc
* contrib docs
* lexicon – terms/def for the docs

#### \[R]espect

* coordination != collaboration

#### \[E]mpathy

feedback guidelines:

* ask, don’t tell
* be specific
* explain yourself
* offer solutions

## Jina Bolton – Living Design Systems

Style guides are awesome!!!

Some things to keep in mind:

* Use a living style guide because it is maintainable
* Naming conventions – use clarity > brevity
* Keep properties organized (doc it, and make sure it is easy to know how to follow)
* Enables rapid dev and testing
* Elements, components, layouts ([modularize](https://ispeakincode.com/#modularize), choose your method or create your own variation)

  * types, states, variations

### LINKS

* <https://github.com/salesforce-ux/theo>
* <http://sfdc-styleguide.herokuapp.com/>
* Responsive design testing (using? not sure what the iframe tool was)

## Conclusion

Camp Sass was awesome! Go next year, you won’t regret it!

[Twitter Tweet](https://platform.twitter.com/embed/Tweet.html?dnt=false&embedId=twitter-widget-3&features=eyJ0ZndfZXhwZXJpbWVudHNfY29va2llX2V4cGlyYXRpb24iOnsiYnVja2V0IjoxMjA5NjAwLCJ2ZXJzaW9uIjpudWxsfSwidGZ3X2hvcml6b25fdHdlZXRfZW1iZWRfOTU1NSI6eyJidWNrZXQiOiJodGUiLCJ2ZXJzaW9uIjpudWxsfSwidGZ3X3NwYWNlX2NhcmQiOnsiYnVja2V0Ijoib2ZmIiwidmVyc2lvbiI6bnVsbH0sInRmd192ZGxfY2hpcnBfMTI3OTQiOnsiYnVja2V0IjoidmRsX29ubHkiLCJ2ZXJzaW9uIjozfX0%3D&frame=false&hideCard=false&hideThread=false&id=584522533245952002&lang=en&origin=https%3A%2F%2Fispeakincode.com%2F&sessionId=2db000740eba09639b54837c8f4cb465dda5e1b5&theme=light&widgetsVersion=1890d59c%3A1627936082797&width=550px)