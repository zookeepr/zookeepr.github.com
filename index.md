---
layout: default
title: 'Zookeepr: Conference Management System'
---

# About

Zookeepr is a conference management system, originally developed for
[linux.conf.au](http://linux.conf.au/).


Zookeepr aims to be a one-stop-shop for your conference management needs. It's
used for guiding the conference experience, from paper review, to delegate
registration and to providing information at the conference.


People who would find Zookeepr immediately useful are organisers of technical
conferences. As the rough edges are smoothed out, we hope that Zookeepr will
fulfill the technical needs of most conferences.


The Zookeepr name comes from the original working title MyLCA, bacronymed to
"Maybe You Like Caressing Animals". The last 'e' from 'Zookeeper' was dropped
to reflect the Web 2.0 aspirations of the project.


If you are a developer or would like more information, please subscribe to our
mailing lists [http://lists.zookeepr.org](http://lists.zookeepr.org) or use IRC
and join us on irc://irc.freenode.org/#zookeepr.

## News

<ul>
  {% for post in site.posts limit: 5 %}
    <li>
      <span>{{ post.date | date_to_string }}</span>
      &raquo;
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>



