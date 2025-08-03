# VarsFromJobname

Sources for my varsfromjobname LaTeX package, available also from CTAN: 

[https://www.ctan.org/tex-archive/macros/latex/contrib/varsfromjobname](https://www.ctan.org/tex-archive/macros/latex/contrib/varsfromjobname "CTAN varsfromjobname")

# Credits

varsfromjobname.sty is based on code by supplied by Friedrich Vosberg, Enrico Gregorio and Markus Kohm, help from Rolf Niepraschk, Sven Naumann, Ulrich Schwarz and Andreas Mathias was greatly appreciated.

# What does this package do?

Using `varsfromjobname.sty` one can easily extract information from the filename, if it follows a certain form. 

The standard LaTeX command `\jobname` returns the name of the LaTeX (master) file. If the filename consists of tokens separated by hyphen we can easily extract certain tokens that can be used _inside_ the document. 

The package expects the filename to be of the form
`one-two-three-four-five-six-seven-eight-nine.tex` and offers the following commands:

* `\getfromjobname{param}`, with `param` in the range of 1 to n (a highlevel
interface to the following commands)
* `\getonefromjobname`
* `\gettwofromjobname`
* `\getthreefromjobname`
* `\getfourfromjobname`
* `\getfivefromjobname`
* `\getsixfromjobname`
* `\getsevenfromjobname`
* `\geteightfromjobname`
* `\getninefromjobname`

# Why can it be useful?


You can use this package for example to define the date of the document in the filename, personally I use it e.g. for `scrlttr2` letters.

# References

* [https://tex.stackexchange.com/questions/212169/qr-code-from-jobname/212171#212171](https://tex.stackexchange.com/questions/212169/qr-code-from-jobname/212171#212171 "QR-code from jobname")

Remark: [egreg](https://tex.stackexchange.com/users/4427/egreg "egreg") gave an improved version of the code written with expl3 which also overcomes the limitation of nine parameters.

* [https://tex.stackexchange.com/questions/116755/timestamp-in-document-pdf-name/116805#116805](https://tex.stackexchange.com/questions/116755/timestamp-in-document-pdf-name/116805#116805 "Timestamp in document / pdf name")

* [https://tex.stackexchange.com/questions/645185/splitting-the-jobname-by-hyphens-in-expl3-syntax "Splitting the \jobname by hyphens in expl3 syntax"]

# Change History

- Version 0.5, as of January 11th 2009: Initial version published

- Version 1.0, published May 2017: 
	- Added various commands which extract necessary information also from included documents
	- Modified code as suggested by egreg

- Version 1.1, published August 2025:
	- Switched to expl3 syntax, allowing more than nine tokens


2025-08-03, Uwe Ziegenhagen 