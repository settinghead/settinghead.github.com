---
layout: post
category : tech
tagline: "Economic & pragmatic URL duplication avoidance solution for web crawlers."
tags : [intro, beginner, jekyll, tutorial]
---
{% include JB/setup %}

## In One Word
A url identifying component for duplication prevention. Used in crawlers. 

## Introduction

Say you want to crawl a whole bunch of web pages, and most of them come from major websites like Blogger and YouTube. In the beginning things are fine, you grab the url addresses and get what you want via Ruby's URL::Open. As time goes on, you begin to find duplicates in your url, like these:

#### Exhibition 1
* http://happy-fake-blogger.blogspot.com/2013/02/o-la-la.html and
* http://happy-fake-blogger.blogspot.com/2013/02/o-la-la.html?#comments
* http://happy-fake-blogger.blogspot.com/2013/02/o-la-la.html?affiliate_track=23243243243

#### Exhibition 2
* http://www.youtube.com/watch?v=9bZkp7q19f0 and
* http://www.youtube.com/watch?v=9bZkp7q19f0
* http://youtu.be/9bZkp7q19f0

In both examples, the three urls essentially point to the same resource (where in Exhibition 1 we can surmise they refer to a blog article, while in Exhibition 2 they all refer to the same music video). 

The problem is we only want one URL for each unique resource. 

## Possible Solutions

(Feel free to comment on things I am not yet aware of. Here it goes. )
* [Detecting Near-Duplicates for Web Crawling]http://www.wwwconference.org/www2007/papers/paper215.pdf
* Use a frequently-updated, exhaustive list to record patterns for common websites

The second solution is what url-identifier goes after.

## url-dentifier

url-identifer is a pragmatic solution that uses very limited resources. 

### Usage

For now, simply add Ruby rules to lib/url-identifer.rb. 

I expect this to change soon as this project gains momentum. Will possibly add a rule table and provide more convenient way for adding & removing rules.