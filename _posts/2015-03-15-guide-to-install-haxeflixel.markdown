---
layout: post
title:  "Guide: How to prepare Haxe and HaxeFlixel"
date:   2015-03-15 14:37:51
description: This is going to be a guide how to prepare Haxe and HaxeFlixel.  
categories:
- Guide
- Haxe
- HaxeFlixel
---

This is going to be a guide how to prepare Haxe and HaxeFlixel. I will show you 
how to install `Haxe` programming language and `HaxeFlixel` game engine on **Windows** and **Ubuntu** operating systems.

## First we need Git
**Windows**<br />
First of all you need to download and install this executable file from [here](http://git-scm.com/download/win). After installation just paste these commands 
into CMD and you're done!
{% highlight bash %}
git config --global user.name "Vardas"
git config --global user.email "El.Paštas"
{% endhighlight %}
<br />
**Ubuntu**<br />
All you need to do is to paste these commands into your terminal!
{% highlight bash %}
sudo apt-get install git-core
git config --global user.name "Vardas"
git config --global user.email "El.Paštas"
{% endhighlight %}

### Now it's time to install Haxe
**Windows** <br />
Just download and install this [file](http://haxe.org/download/)!
<br />
**Ubuntu**<br />
Just copy and paste these commands into your terminal!
{% highlight bash %}
curl http://www.openfl.org/builds/haxe/haxe-3.1.3-linux-installer.tar.gz | tar xvz
sudo sh install-haxe.sh
{% endhighlight %}

###Lime, OpenFL and HaxeFlixel
**Ubuntu and Windows**<br />
To install `Lime`, `OpenFL` and `HaxeFlixel` we will use terminal (*or CMD if you're on Windows*).
{% highlight bash %}
haxelib install lime
haxelib run lime setup
lime install openfl
haxelib install flixel
haxelib upgrade
haxelib install flixel-tools
haxelib run flixel-tools setup
{% endhighlight %}

## You're done!

Yes that was all! You have successfully installed `Haxe` and `HaxeFlixel` on your computer and you're really to code! You can create new project using command below!
{% highlight bash %}
flixel tpl -n "HelloWorld"
{% endhighlight %}