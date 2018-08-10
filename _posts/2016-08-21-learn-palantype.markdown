---
layout: post
title:  "Learn Palantype!"
date:   2016-08-21 17:00:00 -0400
categories: tutorial
tags:
- palantype
- lesson
- howto
- tutorial
- chording
- chorded
- typing
- speed
---

So you want to learn the Palantype (pah-lahn-type) machine shorthand system, do you? Well, you've come to the right (and the only?) place on the Internet. My name is Ted, I'm a developer of Plover, the free open source stenography program. I'm stenoing this guide, not palantyping it. I can't say that I know the system well, but I know enough to get you started. I also don't know how much you know about chording systems or about Palantype itself. I'm going to start from the beginning, and try to be brief. The Palantype is a simple system, simpler than stenography. It's main barrier of entry is the fact that you can't find lessons online for free and you can't get a good Palantype machine for anywhere near what a normal person might consider a "reasonable cost." For that reason, Plover (the software that we'll use to drive the Palantype logic) supports input from regular keyboards that support NKRO.

NKRO simply means that you can press N keys (anywhere from 1 to all the keys on the keyboard) at once and have them register correctly. This is important because while making chords on the Palantype layout, you'll be using many keys and you need them all to get caught by Plover so that it can understand what you are writing. You can read more about the [NKRO keyboards and where to get them on the Plover wiki.](https://github.com/openstenoproject/plover/wiki/Supported-Hardware#keyboards)

## The Layout

The Palantype layout is split across your two hands. Here's a picture from Palantype enthusiast Samuel Belli.

![Picture of a Palantype machine]({{ site.baseurl }}/assets/palantype.png)

Notice how the layout tilts with the hands, and the columns are straight, not staggered, to be more ergonomic than a regular QWERTY keyboard.

Next, we'll see what keys map to what in the Palantype layout. This next picture might raise some questions:

![Palantype layout with key names]({{ site.baseurl }}/assets/layoutlettered.png)

Notice that we have some duplicate keys in this layout. Notice, too, that all the vowels are in the center. This sort of layout may appear as strange, but it's because the Palantype is going to make a syllable, or rather a *sound*, with each stroke. Essentially, there is an order to the keys. After the Palantypist hits all the keys and then lets go, those keys and their order form a sound. Depending on the sound, it may form a word or a part of a word which is then output into the computer.

For example, if the Palantypist hits both `P` keys and the `O` in the center, the resulting raw key representation is `POP` which then translates into the word "pop" on the computer. Now, consider that next the Palantypist hit `L` on the left hand, `A` in the center with their left thumb, and `R` with the right hand, now the resulting raw representation might be `POP/LAR`, which phonetically maps to "popular". And then the output on the computer changes from "pop" to "popular".

### Homerow

The home row of the Palantype is `STFL E U LFTS`

![Diagram of the Palantype home row where the home keys are shaded in]({{ site.baseurl }}/assets/layoutletteredhomerow.png)

### Palan Order

The full palan order is shown by the diagram below:

![Palantype layout with arrows between the keys depicting the phonetic order]({{ site.baseurl }}/assets/palanorder.png)

*Note: the + and ^ keys don't have a phonetic representation but their order in print is consistent.*

All the strokes in raw format that you will see of the Palantype, or if you ever see a paper tape output, will be in palan order:

#### SCPTH+MFRNLYOEAUI^NLCMFRPT+SH

It's important to know this order by heart and be comfortable with it. You can't make a habit of breaking the order in your own strokes or you will end up with a confusing and unpredictable theory.

When representing the order in raw format in this website, we use two additional characters → `-` and `/`:

- The dash (`-`) is used to separate ambiguous keys from each other. For example, the `T` key could refer to either the left T (`T-`) or the right T (`-T`). The dash represents the center of the keyboard.
- The slash (`/`) shows a stroke separator. For words like "popular" where you use two separate chords, we show that they are hit separately with the slash, as in `POP/LAR`. The slash represents the user lifting all his or her fingers off the keys.

### Cross and Point

You may have noticed that there are missing keys on the layout above. You probably also saw the keys that aren't letters. The `+` keys are called "cross" and the `^` keys are called "point". They are used to give an alternate sound for whatever key you are pressing in each section.

- The left cross (`+-`) keys are functionally only one key, they are sometimes split for comfort. If you press it, it changes the sound of the left consonant that you are pressing. For example, if you press `P-`, the beginning sound is "P". If you press `P+-`, the beginning sound is "B".
- The right cross (`-+`) key also modifies the sound of consonants, but for the right hand. So if you press `-P`, the ending sound is "P". But if you press `-P+`, the ending sound is "B". If we take our previous example of `POP` mapping to "pop", then `P+OP+` maps to "bob".
- The point (`-^`) keys are also functionally only one key, and they modify the sound of the vowel being hit by your thumbs. For example, `P+IT` maps to "bit" while `P+I^T` maps to "beet".

### QWERTY to Palan Mapping

If you are using Plover and don't have a Palantype machine, you can still try out these exercises and get started with the theory and lessons. You just need a keyboard that has NKRO. Once you are set up, you can use the Palantype layout on your regular keyboard as demonstrated by this diagram:

![In the QWERTY to palan mapping, S is a, C is q, P is 2, T is w, H is s, cross is z, x, and c, N is 4, L is r, Y is f, O is g, E is v, A is h, U is n, I is b, point is m, comma, period, and slash, L is u, C is j, N is 8, F is i, R is k, M is 9, T is o, the right cross is l, P is 0, S is semicolon, and H is p.]({{ site.baseurl }}/assets/QWERTYtopalanmapping.png)

## The Missing Sounds


| Sound | Produced With |
|---------|-----------|
| B | `P+` | 
| D | `T+` | 
| G | `C+` | 
| J | `+Y` | 
| K | `C` | 
| NG | `N+` |
| QU | `CF` |
| V | `+F` |
| W | `MF-` |
| X | `CS` |
| Z | `S+` |

*Notes:*

- *the C key in the Palantype layout is only hard C. Soft C words just use the S key in most cases.*
- *The Y key can be used for the "Y" sound as well as "ZH" which is the result of words like mea**s**ure and plea**s**ure*

## Vowel Sounds

The vowels are very versatile and some representations are used for phonetic sounds like "ee" and "aye", while others are used for spelling like in "bear" as opposed to "bare"

| Sound | IPA |  Examples | Keys |
|-------|-----|-----------|------|
| a | [æ] | back, shack | `A` |
| ah | [ɑ:] | barn, arm | `A^` |
| ai, one vowel | [eɪ] | mate, game | `E^` |
| ai, multiple vowels* | [eɪ] | feint, faint | `EI` |
| aw | [ɔː] | raw, saw | `O^` |
| e | [e] | peck, met | `E` |
| ee | [i:] | sheet, meek | `I^` |
| ei | [eɪ] | slay, fey | `EI` |
| ea | [i:] | eat, feat, bear | `EA` |
| i | [ɪ] | brick, it | `I` |
| aye | [aɪ] | eye, might | `AI` | 
| o | [ɑ/ɒ] | mock, ox | `O` | 
| oa* | [ɔː] | board, load | `OA` |
| oi | [ɔɪ] | boy, toil | `OI` |
| oo | [u:] | moon, shook | `OU` | 
| ow | [aʊ] | shower, town | `AU` | 
| u | [ʌ] | truck, mud | `U` | 
| ur | [ɜː] | girl, church | `U^` |
| you | [uː] | mute, new | `EU` | 

*\*Using these keys is determined by the sound paired with the spelling of the word.*

## Common Briefs

Briefs are shortcuts for commonly used words.

- `"UFLTS": deletes last stroke`
- `"TH": "the"`
- `"^": "{.}"` the end of sentence period
- `"+-": "{,}"`
- `"+-^": "{;}"`
- `"-^+": "{?}"`
- `"-CS": "{!}"`
- `"+-+": "{:}"`

## Sample exercise

1. The quick brown fox jumps over the lazy dog.
- TH CFIC HRAUN FOCS +YUMPS OEFR TH LE^/+SI T+OC+ ^
