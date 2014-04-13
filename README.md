# Disclaimer

As of the version you are reading, this spec is in early development; do not implement it. Please see the Roadmap section below for details.

# What is this?

A proposal for a standard password changing API.

## Purpose

* Convenience
    * Isn't it always a hassle?
    * In case of security disaster.
* Security 
    * Users will rotate their passwords more often
    * Users might start using password managers more, getting them to make better passwords
    * Semi-automated, scheduled password rotation (requiring master password)

# So what's next?

I would like to get this repository out into the community, get it vetted. Though the idea of authenticating via password over an API shouldn't be too controversial, this is security software, and I would like to know what to fix, or any conceivable reason this is altogether a bad idea. This includes cultural reasons. For instance (as a silly example), if users not used to password managers start using them, will they end up losing their passwords through carelessness more often?

I'm also soliciting pull request from people who have suggestions on what to improve. 

Once it's clear that it's not discouraged by the security heavy hitters, or the community at large, we will roll out V0. If you are interested, and would like to know when it is ready, please email [TODO] or follow @[TODO] and you will be notified when V0 is ready.

# Then what?

My hope is that once this gets solidified, and there is serious momentum behind it, we can start to convince smaller projects and websites to . In particular I'm hoping that the Open Source community will sign on, with projects such as Diaspora, Identi.ca, and Mediagoblin. From there, I will personally solicit some of the members of the startup community in the Silicon Valley area (and I encourage anybody else interested to do the same) who are open to experimentation, to post V0 (a static page, see below). I'm hoping enough good faith assent to the idea will be enough to convince the creators of a few password manager programs to sign on to the idea. We can then start to approach some somewhat larger, more conservative, companies in the area, and have it snowball upwards from there.

# Roadmap

## V0 - Signal of Good Faith

This version will have no functionality. It will just be a JSON file. Serves as a signal that a given website or project is willing to implement V1 once a well used password manager shows interest in implementing it on their end.

The purpose of this is to smooth over the Chicken and Egg problem of getting sites and password managers to get on board. If we can get smaller sites on board, proving it by going as far as to put up a static file, it gets the ball rolling and starts to signal to the password managers that it's something real.

As part of the security deliberations, cleanup of the V1 specification should hopefully be under way, but not complete.

## V1 - Change Password

This will only work on single factor authentication passwords.

* Password requirements for users to see. [todo move to spec, too specific]
* Error field [todo move to spec, too specific]

## V2 - More advanced features

* Two-factor authentication
* Revoke associated tokens

# License

The contents of this repository are licensed under the MIT License.
