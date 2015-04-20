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
- [Git Documentation](http://git-scm.com/documentation)
- [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/)

##Contributing
We're in need of new challenges to help make us a great resource for those looking to learn more about creating and testing web applications. Though, the majority of our current challenges are in Ruby, we're striving to become more language agnostic. Currently, we're looking for new challenges in Python, Ruby, and JS including client-side frameworks like Backbone & AngularJS.

###Submitting your challenge
- Make sure you have a [GitHub account](https://github.com/signup/free)
- Fork the [Challenge Skeleton](https://github.com/paircolumbus/ChallengeSkeleton) on GitHub & follow its format
- Push your changes to a topic branch in your fork of the repository
- Submit a pull request to the repository in the Engineers organization
- We'll review it and close the pull request! Thanks :smile:
