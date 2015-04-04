---
layout: page
title: Challenges
permalink: /challenges/
---

Challenges are marked by difficulty level.

__Beginner:__ Rusty or new to web development, limited knowledge of programming languages & related tools

__Automated Testing:__ A special track for those with an interest in Ruby testing & automation techniques

__Intermediate:__ Very familiar with Ruby, JS, MacOS/Linux, Shell, Git & your text editor of choice.

##Session Drills
__Note:__ Most of these drills are not domain specific and can be completed with the Ruby, Python or NodeJS libraries.

<!-- challenge categories -->
{% for category in site.data.challenges %}
  <h3>{{ category.category }}</h3>
  <p>{{ category.description | markdownify }}</p>
  <ul>
    {% for challenge in category.challenges %}
      <li>
        <a href="https://github.com/paircolumbus/{{ challenge }}">
          {{ challenge }}
        </a>
      </li>
    {% endfor %}
  </ul>
{% endfor %}

##How to submit challenges via GitHub

If you don't have Git or Ruby installed on your computer, please [start here](/getting_started/).

###Submitting Challenges for Review
[![submitting challenges](http://i.imgur.com/6dZYqjx.gif)](http://imgur.com/6dZYqjx)

- Login to your Github.com account
- Fork the challenge that you want to work on from Pair Columbus
- _Clone_ its repo to your computer
- Create a new _branch_
- _Add_ & _commit_ your changes
- _Push_ your changes back to your Github account
- Issue a _pull request_ for your branch from Github

###Documentation
- <http://git-scm.com/documentation>
- <https://www.atlassian.com/git/tutorials/>

##Contributing
We're looking for more challenges! To submit your own for the advancement of others, please check out our section on [contributing](https://github.com/paircolumbus/paircolumbus.github.io/blob/master/CONTRIBUTING.md).
