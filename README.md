# Syllable Counter

![CI Status](https://github.com/Nincodedo/syllable-counter/workflows/CI/badge.svg)

Uses a fallback method—based on the [NLTK readability plugin][nltk] by Thomas Jakobsen <thomj05@student.uia.no> and Thomas Skardal <thomas04@student.uia.no>. This NLTK plugin is itself based on the algorithm implemented in the [Lingua::EN::Syllable perl module][perl] by Greg Fast <gdf@imsa.edu>. Forked from @m09's since archived and now deleted repo.

Thanks to them for making their work available.

[nltk]: https://github.com/nltk/nltk_contrib/blob/master/nltk_contrib/readability/syllables_en.py
[perl]: http://search.cpan.org/~neilb/Lingua-EN-Syllable-0.26/

## Requirements

To use this Java library, you need Java 8 and Maven 3.

## Installation

For previous versions, please refer to the [Maven Central page](https://search.maven.org/search?q=g:eu.crydee%20a:syllable-counter) to find the installation instructions for your build tool or to download the jar directly. Future versions will most likely be deployed to GitHub Maven, but that is yet to be determined.

## Usage

To retrieve the number of syllables of a word, use the `count` method:

```java
import eu.crydee.syllablecounter.SyllableCounter;

...

SyllableCounter sc = new SyllableCounter();
int myCount = sc.count("facility");
// myCount holds 4
```
