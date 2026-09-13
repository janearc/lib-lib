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

- `libreadme` is a package for calibrating a css sheet via a *solver* and also
  has the fun side effect of giving us the ability to create a ci gate bounce
  which can refuse colorways which do not comport with a specific profile,
  which is left up to the user. it has been brought to my attion at least a
  handful of times that this constitutes PHI, and i would argue that is only
  the case if someone wishes to steal your eyeballs, or something like that.
  don't worry about it.
