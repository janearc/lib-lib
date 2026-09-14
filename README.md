# on the nature of these stuff and these things

i have been a person who resides in the shell in unix for a very long time.
one of the things i most love about this environment is it unites people
with a common language. it is, mostly, unbusy, plan, and easily legible.
it also doesn't attempt to monopolize your attention; you have your hands
at the keyboard, you are driving, you tab through what you want, you type,
you know when you submit a form.

your attention is your own. you need not conform to someone else's model for
how you should interact with the world. in this way, i find text-based
interfaces both very human and very humane. they are fundamentally human
interfaces because humans are such incredible users of language, and they
are also humane: they do not control you. they are plain and legible. it is
quite literally in your hands, under your fingers.

i want to share some of the ways i use text interfaces, my relationship with
them, and to come back to where interfaces actually started. with words and
our fingers. we call back to newspapers and presses. the way my terminal is
colored and sectioned is as personal to me as the way a person folds and
carries a newspaper. these are all leaves on an immensely rich tree of human
interaction, made of words.

i don't hate the gui. but i don't need it either.

here's the stuff i want to share.

# owning the libs

it has become clear to me that as i work with presentation layers on various
devices, that it is difficult to say what color i am referring to on a
different platform, regardless of how exact i may be.

accordingly, i have collected a few things here which may be of use.

- `libtheme-css` is a package for representing as precisely as possible a 
  color, and providing a translation layer between these colors. for example,
  if i say that something is 'red', the red on my mac in ghostty will not 
  refer to the red that a different terminal or a web browser or a lamp would
  be. this package attempts to normalize many different color dialects to css,
  which is for sure a questionable decision, but lighting and color spectra
  is not somewhere we may be precise outside of a specific context.

  choices were made, and that's what we do  when we write software.

  to its credit and the author's, libtheme is and likely will remain the world's
  first and only, pre-war chromatic arithmetic library, normalised to css.

  - https://github.com/janearc/libtheme-css

- `libreadme` is a package for calibrating a css sheet via a *solver* and also
  has the fun side effect of giving us the ability to create a ci gate bounce
  which can refuse colorways which do not comport with a specific profile,
  which is left up to the user. it has been brought to my attention at least a
  handful of times that this constitutes PHI, and i would argue that is only
  the case if someone wishes to steal your eyeballs, or something like that.
  don't worry about it.

  generally speaking, we use *libreadme* to calibrate visual expressions
  (text, mainly, but als shapes) in a way that is *legible* first.

  - https://github.com/janearc/libreadme
