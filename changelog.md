# Change log

## v2.1.0 - [Unreleased]

* Python 2 and 3 cross compatibility.
* Allowed "n" to be a syllabic nasal.
* Exposed the `exclude` parameter in various reader methods
  for excluding specific participants. This parameter was implemented at
  pylangacq v0.10.0.

## v2.0.0 - 2016-02-06

* PyCantonese now requires Python 3.4 or above.
* Adopted the CHAT corpus format, piggybacking on [PyLangAcq](http://pylangacq.org/)
* Converted HKCanCor into the CHAT format
* Switched to transparent function names
  (cf. issue [#10](https://github.com/pycantonese/pycantonese/issues/10)): `parse_jyutping()`, `jyutping2yale()`, `jyutping2tipa()`
* Bug fixes: issues
  [#6](https://github.com/pycantonese/pycantonese/issues/6),
  [#7](https://github.com/pycantonese/pycantonese/issues/7),
  [#8](https://github.com/pycantonese/pycantonese/issues/8)
  [#9](https://github.com/pycantonese/pycantonese/issues/9)

## v1.0 - 2015-09-06

* Fixed the Jyutping-Yale conversion issue with "yu"
* Added ``number_of_words()`` and ``number_of_characters()`` for corpus access
* Forced all part-of-speech tags
  (both in searches and internal to corpus objects)
  in caps, in line with the NLTK convention

## v1.0dev - 2015-09-02

* Overall code restructuring
* Only Python 3.x is supported from this point onwards
* Used generators instead of lists for corpus access methods
* Added the part-of-speech search criterion
* Added Jyutping-to-Yale conversion
* Added Jyutping-to-TIPA conversion
* Disabled the function for reading a custom corpus dataset (it will come back)

## v0.2.1 - 2015-01-25

* Fixed corpus access path issues

## v0.2 - 2015-01-22

* [The Hong Kong Cantonese Corpus](http://compling.hss.ntu.edu.sg/hkcancor/) is included in the package.
* A general-purpose ``search()`` function is defined, replacing the
  element-specific search functions from version 0.1.

## v0.1 - 2014-12-17

* Basic functions available, including...
* Parsing Jyutping romanization
* Reading a tagged corpus data folder
* Searching by a given element (onset/initial, nucleus, coda, final, character)
* Searching by a character plus a range
