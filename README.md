MultiRegExp
===========

A simple java-script object which allows you to get the text and string location of many groups within a regular expression.


USAGE
=====
var exp = new MultiRegExp(/([a-z]+)(?:\s|\_)*([0-9]+)/i);<br>
exp.exec("test_53");  //will return {0: {index:0, text:'test'}, 1: {index:5, text:'53'}}


Note: 
  -This requires that capture groups are not nested use (?:...) when bracets around unneeded blocks are required.
  -Repitition of capture groups is not permitted as regular expressions only return one of the matched capture groups in the repetition use ((?:match)+) instead.
