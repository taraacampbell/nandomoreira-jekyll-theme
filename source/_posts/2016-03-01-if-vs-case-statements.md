---
layout: post
title: "If Versus Case Statements"
date: 2016-03-01 09:00:20
comments: true
description: ""
keywords: ""
categories:
- welcome
tags:
- welcome
---

If statements are very similar to case statements, and have the same functionality. The only real difference is their performance in a program. Case statements are slower to run in comparison to if statements. Sometimes the difference in time is often in microseconds, but to some this discrepancy is important.

Both if statements and case statements are ways to compare values, whether it be integers, floats, or strings. If statements are lengthier, and use the conditional “==” operator to compare values, while case doesn’t need this operator. Case implicitly uses “===” in its code, because the word “when” substitutes the need for an operator. For an example, a case statement reads:


letter = gets.chomp
case letter

when “x”, “y”, “z”
	puts “you’re at the end of the alphabet”
when “a”, “b”, “c”
	puts “you’re in the beginning of the alphabet”
else
	puts “you’re in the middle”
end


Whereas in an if statement, it would read like this:


letters = gets.chomp

if “x”, “y”, “z”=== letter
	puts “you’re at the end of the alphabet”
elsif “a”, “b”, “c”=== letter
	puts “you’re in the beginning of the alphabet”
else
	puts “you’re in the middle”
end


As you can see, the differences are only in characters, so why would you use one or the other? Well the triple equals, “===” is hidden in the case statement. It is used to compare things to see which group it belongs to. It is called on the when statements, not on the case definition, so often coders can more specifically define things.

Some coders prefer if statements not only because of their speed, but because it’s much easier to add another “when” to a case statement than it is to add another conditional to an if statement. If another “when” is added by someone else looking at their code, it can create more branches to an already complicated code.


http://www.skorks.com/2009/08/how-a-ruby-case-statement-works-and-what-you-can-do-with-it/
http://www.daniellesucher.com/2013/07/ruby-case-versus-if/
https://www.ruby-forum.com/topic/4404937
http://mauricio.github.io/2011/05/30/ruby-basics-equality-operators-ruby.html


