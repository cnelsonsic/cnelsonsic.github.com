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

1. Toys are stored in the [traditional plastic capsule](http://www.candymachines.com/Empty-Vending-Capsules-C99.aspx),
    usually 1-2 inches around.
2. The capsules are stored in a hopper at the top of the machine, usually in a
    clear plastic or glass container.
3. At the bottom of the hopper is an opening a touch bigger than the capsules.
    The opening is at the far back of the mechanism.
4. Underneath that is a disk which rotates when the crank is turned.
5. The capsules rest on top of the disk. It has a circle cut out, where when it
    matches the upper opening, the capsule drops down into a chute and rests on
    a third disk, which is attached to the same shaft as the second disk.
5. The third disk has a hole cut opposite the first disk's, but as the disks
    turn, the chute is closed off from other capsules, and the bottom of the
    chute opens to release the capsule.
6. Finally, it slides down a curved chute to the excited <del>customer</del>
    child who is eagerly cranking the handle.

Pictures, animations and a .blend file will be along shortly.

Funds Acquisition Mechanism
---------------------------

Right now, I have no ideas about how to take money and allow or not allow turning of the crank.
I would like to keep it 3d-printable, but I have no ideas for this at the moment.

However, there are [electronic coin validators](http://www.adafruit.com/products/786)
which could be hooked up to an arduino, and disengage a rachet that would
otherwise prevent turning the handle.
