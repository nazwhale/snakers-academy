# Snakers Academy

We're going to make the retro phone game Snake with Ruby (a programming language) and Gosu (a 2D game development library).

### Why Ruby?
Ruby is one of the most minimal, readable and versatile coding languages out there, making it a great one to get started with. The fact it's so easy to use means you'll be able to start writing working code asap.

It's also decent for jobs (the [Ruby on Rails framework](http://rubyonrails.org/) is widely used professionally).

My personal opinion on choosing a coding language to start with is that it really doesn't matter that much. Just pick one and get going. The core concepts of coding remain consistent through most languages. The most important thing is to start playing, building things, and thinking like a coder asap.

### Setup

##### Get a text-editor

There are lots to choose from, and developers love to argue over which one is best (just like they love to argue which language is best).

Just get [Atom](https://atom.io/). It's easy to use, looks nice, and is made open-source by [GitHub](https://github.com/) (a.k.a the Citadel of Ricks).

##### Install Homebrew, Ruby, and Gosu

Mac
* Install [Homebrew](https://brew.sh/), Ruby, and  [SDL2](https://github.com/gosu/gosu/wiki/Getting-Started-on-OS-X) by running the following commands in the terminal.

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

brew install ruby

brew install sdl2

gem install gosu
```

Windows
* Install [Ruby](https://rubyinstaller.org/)
* Install [RubyGems](https://rubygems.org/pages/download/
* Install [Gosu])(https://www.libgosu.org/ruby.html): `gem install gosu`

Linux
* Instructions [here](https://github.com/gosu/gosu/wiki/Getting-Started-on-Linux)

### Get started

* Clone or download this repository
* Navigate to `snakers-academy` using the terminal, and run the program
```
cd snakers-academy
ruby play.rb
```
### What next?

If you need some guidance on what approach to take, check out this [plan of action](https://github.com/nazwhale/snakers-academy/blob/master/plan_of_action.md) I've sketched out.

Once you have a working snake game, see if you can complete some of the challenges listed [here](https://github.com/nazwhale/snakers-academy/blob/master/challenges.md) 🐍

### Further resources

Learn Ruby basics
* [Chris Pine's 'Learn to Program'](https://pine.fm/LearnToProgram/chap_00.html) is, in my opinion, the best intro out there (super friendly and not too long). At one point you build a tamagotchi, which made me happy
* Completing katas on [Codewars](https://www.codewars.com/) is a great way to train your brain

Funky things to do with Ruby
* [Gosu tutorial](https://github.com/gosu/gosu/wiki/Ruby-Tutorial)
* [Sonic-pi](http://sonic-pi.net/)

Other
* [Daniel Shiffman's YouTube channel](https://www.youtube.com/user/shiffman): Creative coding tutorials in JavaScript by the most enthusiastic man in the world

### Acknowledgements
Thanks to [Joel Walden](https://github.com/joelwalden/ruby-snake), who's code was adapted for this tutorial, and [Makers Academy](http://www.makersacademy.com/), for putting on the event.
