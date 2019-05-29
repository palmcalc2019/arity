# Arity

`org.javia.arity` 'Arity' is an arithmetic engine for for Java, created by [Mihai Preda](https://github.com/preda) between 2003 and 2009.

Originally a [Freshmeat project](http://freshmeat.sourceforge.net/projects/arity), the project was apparently moved to Google Code some time after 2008. There are no working links for the Google Code URL; apparently it was excluded from the Google Code archive.

The code was imported from google code several times, by several different people. The most notable imports are:

* [By the original author in 2014](https://github.com/preda/arithmetic). The project was renamed to Arithmetic, then seemingly reabandoned. Uses an obscure python build system `setup.py`.
* [By Hoijui in 2016](https://github.com/hoijui/arity). This version includes a standard Maven pom.xml, and successfully builds [as of this writing](https://github.com/hoijui/arity/tree/00cffe65b821041eecaa4e3fbb176251714afdc7).
* [A fork from Preda's version by piusvelte](https://github.com/piusvelte/arithmetic), which includes original work to fix precision errors by using Java's BigDecimal API
* [A fork from Hoijui's version](https://github.com/Cmdmac/arity) also includes original work to fix mathematical errors; but the comments & commit messages are in Chinese, so this was overlooked at first.

This repo is based on [Cmdmac's](https://github.com/Cmdmac) [fork](https://github.com/Cmdmac/arity).

It's for use in the PalmCalc 2019+ Android app, a revived version of Cybrosys's PalmCalc.

Future & Maintenance
-----

I am a programmer, not a mathematician. I know about maintaining & updating build files, correcting logical errors in code. That sort of thing.

**I don't know how to add mathsy features to this project!**.

As such, no development work will be done to this code.
Just build & maintenance stuff.

I just need a guaranteed place to get this dependency from, for another legacy app.

I do accept pull requests, though.

TODO
----

Also include the [improvements done by piusvelte](https://github.com/piusvelte/arithmetic/commit/5fb74edd2ca32401a93dcbae215a155c1693bd27)

## Use

	mvn package
	java -jar target/arity-*.jar
	java -jar target/arity-*.jar "1+2"
