# toki wile 0.0.4

toki wile is a conlang that combines the parts of Ithkuil I find interesting with the parts of Toki Pona I find cute and learnable. This document, for now, assumes familiarity with Toki Pona and maybe some familiarity with Ithkuil.

I made this because I want to play with it, and find out what the interesting parts of Ithkuil feel like in a cute and learnable context. Maybe it's a lot of fun! Maybe it doesn't work at all! If you're interested, [**join the toki wile Discord**](https://discord.gg/bBcnEbxA9C).

Ithkuil is [©2004-2021 by John Quijada](http://ithkuil.net/). Toki Pona [was invented by Sonja Lang](http://tokipona.org/).

## Phonology
It's like toki pona (aeiou ptksjnlmw), but with consonant clusters and geminated consonants.

w/j do not appear in coda position, and instead there are diphthongs (`au ai eu ei oi`). Other vowel pairs like `ea` are disyllabic.

Stress is on the first syllable of each word.

/w/ has the allophone \[f\~v\] before /u/, and /j/ has the allophone \[ç\~ʝ\] before /i/.

## Words and sentences 
There are two kinds of words: **pronouns** and **formatives**.

Formatives have an Ithkuil-like fusional slot structure, and are further divided into **nouns** and **verbs**.

There are no particles. Instead, there's a case system (replacing `li`, `e`...) and a "namako" formative slot (replacing `ala`, `anu`...)

The sentence structure is:

    ((Nla) Vla) (N0)   (V1 N1) (V2 N2) (V3 N3)...
    ↑           ↑      ↑       ↑       ↑
    la-clause   head   tail    tail    tail...

`N0` is called the "head", and each `Vi Ni` is called a "tail". The meaning is basically:

    (When / Given that "Nla Vla":)  <-- optional
          "N0 V1 N1",
      and "N0 V2 N2",
      and "N0 V3 N3"...

That is, the nouns in the head `N0` "distribute" over all the verb-noun "tails". This is a generalization of the toki pona `S li V1 O1 li V2 O2`.

If present, the "la-clause" offers a clausal "context" or "condition" for the whole sentence. Its presence is marked by a verb ending in `-a` (see "Illocutions").

If there are no tails, then the nominative-case nouns in the head are linked copula-wise, "N1 is N2 (and is N3...)". So, it's a bit easier to distinguish "I eat" and "I am food" in toki wile.

## Pronouns
These are modeled after Ithkuil's PRAs. The shape is either C(C…)V, or VCCV. (When I use something like "VCCV" to describe the shape of a word, that means "vowel, consonant, consonant, vowel".)

The consonants indicate pronoun roles, and the vowels indicate cases.

    m - mi
    s - sina
    n - ona
    l - ni (demonstrative)
    t - "ni:" (next sentence)
    k - seme?

For example, `mi` is "mi li" (`-i` marks the nominative case), and `se` is "e sina" (`-e` marks the accusative case).

A consonant cluster combines referents: `sne` is "e sina e ona".

The VCCV shape rolls two pronouns into one funky word. `esmi` means the same thing as `se mi`. This is just an aesthetic thing from Ithkuil I like.

## Formatives
These are the building blocks of the language: nouns and verbs.

As in Ithkuil, the structure is divided into consonant/vowel "slots":

    (Vn +) (preverbs +) Cr + Vs + Ca (+ suffixes) + Vk

### Required slots
The **Cr** slot is the root, found in the lexicon. For example **sk** means "lukin / kule".
Each root in groups two content words from toki pona, called its two "stems".

The **Vs** slot selects a stem from the root, and marks whether this formative is a noun or verb:

    -a-   Stem 1, noun.
    -e-   Stem 2, noun.
    -au-  Stem 1, carrier noun. The next word is a name. (laule Lin = "e jan Lin")
    -eu-  Stem 2, carrier noun. The next word is a name. (leule Kiti = "e soweli Kiti")
    -o-   Stem 1, verb.
    -u-   Stem 2, verb.
    -i-   Pronoun: interpret Cr as a pronoun. This allows applying namako, Ca, suffixes... to pronouns. (omitwe = taso-RPV-KLP-ACC)

The **Ca** slot says some things about the "configuration" of the noun or of the event described by the verb. It is described in its own section below.

The **Vk** slot marks case for nouns, and illocution for verbs. See the tables below.

### Vn
Vn is an initial vowel that I stuffed random bits of meaning in. The n stands for namako!!!

    a-  "ala" on verbs.  also on nouns: "I ate not-the-bread (implied: but I ate something else)".
    e-  no meaning, use when an initial consonant cluster is too spicy
    i-  "kin" (also), on any formative
    o-  taso (only), on any formative
    u-  anu, on any formative, links disjunctively with previous formative.

### Preverbs
You can put as many of these as you want in front of the root slot. They behave exactly as in Toki Pona. They're not currently allowed in a noun.

    -wa-  kama...
    -wi-  wile...
    -we-  awen...
    -wo-  sona...
    -wu-  lukin...
    -je-  ken...
    -jo-  open...
    -ju-  pini...

### Suffixes
The **suffixes** are each of the form "VxCx", where "Cx" is a root from the lexicon and "Vx" marks how it applies:

    -a-  Stem 1, modifier.
    -e-  Stem 2, modifier.
    -o-  Stem 1, modifier, as if preceded with "pi".
    -u-  Stem 2, modifier, as if preceded with "pi".
    -i-  Ca stacking.

This is the equivalent to compounds in Toki Pona. As an extra feature taken from Ithkuil, a "pi" on the last item marks that the modification of the root concept is "incidental" (like "jan pona = good person"), whereas its absence marks that the modification is "lexicalizing" (like "jan pona = friend").

    lale    "e jan"           (the person)
    lalape  "e jan pona"      (the friend)
    lalope  "e jan pi pona" ! (the good person)

The vowel -i- is used to stack/nest Ca configurations. For example, `lalwe` (group of people) can become `lalwilje` (a pair of groups of people).

If the consonant cluster in a suffix is -st-, it is a case accessor suffix. This always makes a noun even if Vs marks verb status.

    -ist  "one who V-s"
    -est  "one who is V-ed"
    -ust  "haver of N"
    -ast  "context for N or for doing V"
    -aust "goal of N, purpose of V-ing"
    -eust "what is used by N, or used for V-ing"
    -ost  "place where N is, or where V-ing happens"
    -east "manner of V-ing"
    -aist "similar to N, or what V-ing is done like"

## Cases
These mark the role of the noun in the sentence.

    -i   nominative, subject (tp: li)
    -e   accusative, object (tp: e)
    -u   genitive (scopes on the previous word. covers one sense of pi)
    -a   X la (as in "tenpo pini la". see -a illocution)
    -au  tawa X
    -eu  kepeken X
    -o   lon X
    -ea  tan X
    -ai  sama X
    -oi  "o!" (vocative)

The "genitive" is really a broad appositive case, not limited to "genitive" in the Ithkuil sense.

## Illocutions
Illocution marks whether this verb is an assertion, question, command...

Also, for assertions, it marks evidentiality (the source of the information you're asserting).

    -i   "mi lukin / mi pali"
           I'm asserting this based on direct, present, outside experience.
           This includes statements about what I'm doing.

    -o   "mi sona"
           I'm asserting this based on indirect knowledge.
           Memory, hearsay, hunches, conventional wisdom...

    -e   "mi pilin"
           I'm stating my opinion or internal feelings.

    -oi  "o!" (hortative)
           Not an assertion: I'm expressing a wish that things be this way,
           or a command for the listener to make things be this way,
           or (with "moi") expressing that I should make it be this way.

    -ai  performative
           This is true by virtue of me saying it's hereby true!
           For example, "I hereby apologize" or "I hereby greet you" (=hello).

    -u   "anu seme?"
           Marks a question. Yes/no, or wh-question if there's a -k- pronoun.

           By the way, you can use "nwo-" (lon) to answer yes/no questions,
           or you can repeat the verb. Either way, you should probably copy
           the Ca from the question verb, and use appropriate evidentiality.

    -a   marks la-clause
           Not really an illocution, just marks the end of Vla.
           See "Sentence structure".

## Lexicon
I've only listed the toki pona content words associated with the two stems.
* When used as a root in a noun formative, these have the toki pona noun meaning.
* When used as a root in a verb formative, these have the toki pona verb meaning.
* When used as a suffixes, these have the meaning they have as toki pona modifiers in compounds.

An entry like `-PL- olin, suwi` means: pla- is olin/noun, ple- is suwi/noun, plo- is olin/verb, plu- is suwi/verb.

```
    -P- pona, epiku
    -PP- suli, lili
    -PK- pu, ku
    -PL- olin, suwi
    -PJ- sijelo, unpa
    -PS- seli, lete
    -PW- wawa, lape
    -T- toki, sitelen
    -TJ- pali, pana
    -TL- ilo, kepeken(?)
    -TM- mani, esun
    -TT- tan, nasin
    -TP- lipu, poki
    -TW- tenpo, awen
    -TS- open, pini
    -K- ike, jaki
    -KJ- pakala, utala
    -KK- moli, kipisi
    -KL- kute, kalama
    -KW- kiwen, ko
    -KS- musi, nasa
    -S- pilin, sona
    -SK- lukin, kule
    -SM- sama, tonsi
    -SP- walo, pimeja
    -SPJ- loje, jelo
    -SPW- laso, unu (purple)
    -SW- wile, alasa
    -SJ- ijo, kulupu
    -SS- jo, lanpan
    -ST- (marks case accessor suffix)
    -STJ- (marks inverse case accessor suffix)
    -N- nanpa, nimi
    -NJ- wan, tu
    -NL- linja, len
    -NN- mute, ale
    -NS- insa, selo
    -NSJ- sinpin, monsi
    -NP- anpa, sewi
    -NT- ante, monsuta
    -NTS- jasima, /
    -NK- lawa, poka
    -NW- lon, weka
    -L- jan, soweli
    -LJ- kala, pipi
    -LW- akesi, waso
    -LK- kasi, kili
    -LKJ- soko, /
    -LNSKW- kijetesantakalu, /
    -LL- telo, kon
    -LN- luka, noka
    -LT- oko, uta
    -M- ma, tomo
    -MW- tawa, kama
    -MJ- moku, pan
    -MK- misikeke, 
    -MP- nena, lupa
    -ML- mije, meli
    -MS- suno, mun
    -MT- sike, leko
    -MM- mama, /
    -Č- yupekosi, /
```

## Ca
It's the fun part of Ithkuil! Here's a table.

```
   Extension   Perspective   Pronoun   Configuration
   =========   ===========   =======   =============
   ALE:  Ø     NRM: l²       (see ¹)   WAN:    Ø
   INSA: s     RPV: t                  TU:     j
   OPEN: k     N:   n                  KLP:    w
   PINI: p

   ¹ A "pronoun infix" in Ca is allowed *only when Ext is Ø*.
       * On a noun, they express a genitive: lenmwe = "lenwe mu", twallo = "twalo lu"
       * On a verb, they express a subject: pwusni = "ni pwusi"
   ² NRM -l- is omitted if preceded by non-null Ext or before pronoun "m".
     This is equivalent to applying the substitutions sl→s kl→k pl→p lm→m.
```

(The order these apply in to a root is: Configuration → Extension → Perspective. What that boils down to is that -stw- means "some part of a hypothetical group", not "a hypothetical group of middle parts".)

### Extension
* ALE (Ø) describes a whole thing.
* INSA focuses a middle or part of something. For verbs, it acts like a continuous tense.
* OPEN focuses the start/head of something. For nouns, this might be the source of a river or the entryway of a house — interpretation is a bit creative.
* PINI focuses the end of something. For nouns, this might be like the last bit of food left, or the butt of a cigarette.


### Perspective
* NRM describes a real specific instance.
* RPV describes a hypothetical, unspecific, imagined instance. On verbs, it's like a subjunctive.
* N describes general claims, like "birds fly" (as a rule). It makes "kinds" out of nouns (a bird → "birds in general") and acts like a gnomic aspect for verbs.

### Configuration
* WAN describes "one thing" at a time: one bird, or many birds each in isolation.
* TU describes a pair acting/occuring together, or many pairs each in isolation.
* KLP (kulupu) describes a group acting/occuring together, or many groups each in isolation.

The point here is that configuration is not pluralization. In Ithkuil terms, the distinction between Monadic and non-Monadic is unmarked. So, `lweli` means "a bird" or "birds (a bird here, a bird there)", while `lwelwi` means "a flock of birds" but also "flocks (a flock here, a flock there)". You can use suffixes -anj (one) or -ann (many) to be more explicit about number.
