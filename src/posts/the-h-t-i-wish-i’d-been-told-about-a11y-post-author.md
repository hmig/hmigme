---
layout: layouts/post.njk
title: "The $h!t I Wish I’d Been Told About #A11y Post author"
date: 2015-05-06T03:41:54.341Z
---
Almost a year ago, I attended [JSConf](http://2014.jsconf.us/). It was amazing. I left that conference with SO many great takeaways, the biggest and most challenging for me was web accessibility.

For a few days following the event, I kept finding myself thinking more and more about how users that were blind, visually impaired, deaf, motor-impaired and so on would use the thing that I was working on. I was visualizing these people in my head struggling over the the most basic aspects, and suddenly it became real for me. I could see how bad the user experience was and I wanted to fix it ASAP!

But, where should I start? So, I turned to the internets and sought out to find the go to resources for web accessibility.

## Step 1.: Audit the site

1. [W3C validate](https://validator.w3.org/) (this will help you fix heading errors, ect)
2. Navigate the site strictly via tab. Can you tab logically and easily? If not, note where/how/why to fix.
3. Automated tests. (ATs)

   * I use gulp, so lean towards using [gulp-a11y](https://www.npmjs.com/package/gulp-a11y) (free)
   * There’s also [tenon.io](https://www.npmjs.com/package/gulp-tenon-client) ($$)
   * I like running updated pages through [WAVE](http://wave.webaim.org/report#/ispeakincode.com). It’s not automated, but, I find the info regarding the errors helpful.
4. **Repeat 1-3 until no more errors**. Seriously, do not pass ‘GO,’ do not collect $200. Do not move forward until your site passes these tests.

Some of my gotchas that made it to production for a sprint (or few):

* [The first rule of aria…](https://twitter.com/zeldman/status/586200719088193537) – It seems as though #a11y newbies (me included) get aria-happy, the ATs will help catch errors here. Another good article on aria: [HTML5 Accessibility Chops: notes on using ARIA](http://www.paciellogroup.com/blog/2012/06/html5-accessibility-chops-using-aria-notes/).
* Just because you have alt tags, doesn’t mean they are good ones. I had issues with alt text being the same as the text below the image. Sometimes it is ‘ok’ to have alt=” “. ATs will point this out too.
* Out of order headings h1, h2, h4 … but no h3. 🙁

## .: Knowing Where To Go For Help/Info

### Information

* [WebAIM](http://webaim.org/intro/)
* [A11Y Project](http://a11yproject.com/)

  * [Checklist](http://a11yproject.com/checklist.html)
* [The Paciello Group](http://www.paciellogroup.com/)
* [Web Accessibility Course](https://webaccessibility.withgoogle.com/course) by Google
* [Karl Groves](http://www.karlgroves.com/)‘ website
* [ARIA Examples](http://heydonworks.com/practical_aria_examples/) by [@heydonworks](https://twitter.com/heydonworks)
* [Census Info](http://factfinder2.census.gov/faces/tableservices/jsf/pages/productview.xhtml?pid=ACS_12_1YR_S1810&prodType=table) (helpful when trying offer data/statistics on the population impacted by accessibility needs)

### Social

* Twitter: [\#a11y](https://twitter.com/hashtag/a11y?f=realtime&src=hash)
* [Slack](https://web-a11y.slack.com/messages/general/)
* [Accessibility Wins](http://a11ywins.tumblr.com/) on tumbler – a curated list of sites implementing specific features for accessibility

### Testing

* [Wave](http://wave.webaim.org/)
* [gulp-a11y](https://www.npmjs.com/package/gulp-a11y)
* [Tenon](http://www.tenon.io/#testnow)
* [How to: Voiceover](http://webaim.org/articles/voiceover/)
* Developer tools in chrome and FF
* [Google’s Complete List of Accessibility Tools](http://www.google.com/accessibility/all-products-features.html)
* [Toolbar for IE 9+](http://www.paciellogroup.com/resources/wat/)
* Screen Readers

  * [JAWS for Windows (free 40 min. demo version)](http://www.freedomscientific.com/downloads/jaws/jaws-downloads.asp)
  * [NVDA for Windows (free)](http://www.nvaccess.org/download/)

### Frameworks

* Bootstrap

  * [Assets Framework](http://assets.cms.gov/resources/framework/3.0/Pages/) by the government based on bootstrap
  * [Paypal](https://github.com/paypal/bootstrap-accessibility-plugin)
* [Angular](https://docs.angularjs.org/api/ngAria)
* WordPress: [themes](https://wordpress.org/themes/tags/accessibility-ready/) | [plugins](https://wordpress.org/plugins/wp-accessibility/) | [group](https://make.wordpress.org/accessibility/)
* [iCheck](http://fronteed.com/iCheck/): Accessible checkboxes and radio buttons using jQuery

### Transcriptions

* [Verbalink](http://verbalink.com/)
* [Speechpad](https://www.speechpad.com/)
* [Rev](https://www.rev.com/transcription)

Some history behind me writing this post. It took me a year to get to the point where I could say, confidently, I know where to look for good info on this topic.

And, here’s what I’d like to call my “Don’t do what I did” list (a.k.a. – chasing your tail around until you’re dizzy):

1. [The w3c](http://www.w3.org/TR/wai-aria/) – I love you, but I can’t read these docs without a constant drip IV of caffeine and a shock treatment for every time I fall asleep. (Of course I reference the w3c for accuracy, but NOT for how-to’s.) They, also, have a lot of content via the [web accessibility initiative](https://www.w3.org/WAI/intro/accessibility.php), but again…so much content/reading, yet, so few examples.
2. [MDN](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA#Examples) – In fairness, it looks like there have been a lot of updates here. When I was originally here, there were pages that were like… (╯°□°）╯︵ ┻━┻) f-this. No one can agree on best practices and until they do, we are not dealing with documentation. But, it’s still a cluster-mess if all you are trying to do is figure out how/where to get started.
3. Finally – I was like… I just want examples!!! Someone, please, just show me some freaking examples!!! So, I went to see what the frameworks (bootstrap/foundation/ect) did for accessibility. Unfortunately, at the time, I was finding nothing, zero, zilch…However, I did find bootstrap plugins and forked repos that were accessible. I was so frustrated to see that these existed, but they were not being brought back to the main codebase:

   * [Assets Framework](http://assets.cms.gov/resources/framework/3.0/Pages/) by the US government
   * [Paypal Plugin](https://github.com/paypal/bootstrap-accessibility-plugin) for the components.

Things on #3’s front are changing, as well, for the better and you now see some [basic info in the docs](http://getbootstrap.com/getting-started/#accessibility). They even point out their color contrast flaws.

So, I was running into all these issues trying to find a good place to start. Eventually, I found [Marcy Sutton’s](http://substantial.com/blog/2014/07/22/how-i-audit-a-website-for-accessibility/) article on how to audit a site for accessibility. YAY!