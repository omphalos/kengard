kengard
=======

Bare-bones
[spaced repetition](https://en.wikipedia.org/wiki/Spaced_repetition_system)
web app focused on speed drills.

Normally I use
[Anki](http://ankisrs.net/)
for spaced repetition learning.
I think Anki's great
but I wanted to try an app that is focused on speed drills.

Instead of a typical spaced repetition algorithm,
kengard works by measuring your time-to-correct-answer
and using a
[Bayesian bandit](https://github.com/omphalos/bayestian-bandit)
to choose what card to show next.
I thought this might be a simple and effective way
to get a randomized spaced-repetition effect
while incorporating speed into the algorithm.

Data Storage
============

Cards are loaded from cards.json
(which you can replace with your own set of cards)
and the user's progress
is stored in localStorage.

Quick Start
===========

Clone the repo, and:

    npm install

Then run your favorite static file server, such as:

    python -m SimpleHTTPServer
