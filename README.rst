Flickr Pony 
===========

.. image:: https://api.travis-ci.org/ZuluPro/flickr-pony.svg
        :target: https://travis-ci.org/ZuluPro/flickr-pony

.. image:: https://coveralls.io/repos/ZuluPro/flickr-pony/badge.svg?branch=master&service=github
        :target: https://coveralls.io/github/ZuluPro/flickr-pony?branch=master

This library provides a `Django Storage`_ for use `Flickr`_ in read and write
operations.

With 1To free and a thumbnail system, Flickr is a quite good solution for store
wide pictures in original format and retrieve them in smaller format

As Flickr is dedicated to photos/images, it is not a conventional
object-storge, we consider all pics from all users in the same bucket but
different directories. So what should a be directory path on other storages
will be a user ID in this one.


Docs
====

Comming...


Settings
========

**api_key** : Findable at
`https://www.flickr.com/services/apps/create/apply/`_, it is the only one
mandatory data for read operations.

**api_secret** : Given with the API KEY

**oauth_token_secret** : Oauth access token, not request token

**oauth_token_secret** : Oauth access token secret, not request secret

**user_id** : Your personal User ID, findable at your Flickr web page.
It is the last part of URL example: ``140893176@N07``. This data is useful
if you want to automatize action related to this user.

.. warning::
    Get all authentication info may be really long and boring, we advise you
    this page http://acme.com/flickr/authmap.html

Contributing
============

All contribution are very welcomed, propositions, problems, bugs and
enhancement are tracked with `GitHub issues`_ system and patch are submitted
via `pull requests`_.

We use `Travis`_ coupled with `Coveralls`_ as continious integration tools.

.. _`Django Storage`: https://docs.djangoproject.com/en/1.9/ref/files/storage/
.. _`Flickr`: https://www.flickr.com
.. _`GitHub issues`: https://github.com/ZuluPro/flickr-pony/issues
.. _`pull requests`: https://github.com/ZuluPro/flickr-pony/pulls
.. _Travis: https://travis-ci.org/ZuluPro/flickr-pony
.. _Coveralls: https://coveralls.io/github/ZuluPro/flickr-pony