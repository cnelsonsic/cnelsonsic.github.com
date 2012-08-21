---
layout: post
title: "DIY Gashapon"
tagline: ""
description: "Notes about the design of my diy gashapon machine."
category: diy
tags: [diy, 3d, weeaboo]
---
{% include JB/setup %}

So, I wanted to build a vending machine.
----------------------------------------

I've always liked those little awful 25¢ vending machines, they were always
such a magical little boxes, full of plastic garbage that's not worth the time
it takes to turn the crank.

Japan has a neat thing called [Gashapon](http://en.wikipedia.org/wiki/Gashapon).

It's basically a high-end vending machine, priced anywhere from $1 to $6, and
actually containing good-quality goodies.

So, a few months ago, I had the idea to put together my very own gashapon machine,
mostly as an interesting showpiece for my living room or desk at work.

Plastic Capsule Dispensing Mechanism
------------------------------------

The first challenge to overcome was the actual dispensing mechanism.
Considering that I'm a software engineer and not a mechanical engineer,
the level of engineering that I'm capable of is roughly "rube goldberg" level.

After a few iterations, I came up with a "will-probably-work" mechanism.

It functions roughly like this:

Toys are stored in the [traditional plastic capsule](http://www.candymachines.com/Empty-Vending-Capsules-C99.aspx),
usually 1-2 inches around.
The capsules are stored in a hopper at the top of the machine, usually in a
clear plastic or glass container.
At the bottom of the hopper is an opening a touch bigger than the capsules.
The opening is at the far back of the mechanism.
![](/gashapon/1.png)

Underneath the bottom of the hopper (Green in these images) is a disk (pink),
which rotates when the crank is turned.
![](/gashapon/2.png)

The capsule rests on the solid parts of the disk, until it is turned and lets
the capsule drop through.
![](/gashapon/3.png)

The capsule drops down into a chute and rests on a second rotating disk, which
is attached to the same shaft as the first disk.
![](/gashapon/5.png)

The second disk is set exactly opposite of the first, so that the capsules'
downward path is interrupted.
![](/gashapon/6.png)

As a side effect, additional capsules are prevented from falling by the first
capsule being there, as well as the first disk separating the two as the
second disk opens the path downward.

As the disks continue to turn, the opening below opens and releases the capsule
into a chute below.
![](/gashapon/9.png)

A more realistic rendering of the mechanism:
![Animated Capsule Dispensing Mechanism demonstration](/gashapon/gashapon.gif)

Funds Acquisition Mechanism
---------------------------

Right now, I have no ideas about how to take money and allow or not allow turning of the crank.
I would like to keep it 3d-printable, but I have no ideas for this at the moment.

However, there are [electronic coin validators](http://www.adafruit.com/products/786)
which could be hooked up to an arduino, and disengage a rachet that would
otherwise prevent turning the handle.
