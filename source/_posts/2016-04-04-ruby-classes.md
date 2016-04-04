---
layout: post
title: "Ruby Classes"
date: 2016-04-04 09:00:20
comments: true
description: ""
keywords: ""
categories:
- welcome
tags:
- welcome
---

Classes in ruby are helpful to create multiple objects with the same basic format. If you want five different cakes, they all have the same attributes including the cake, frosting, filling, writing, size, etc. It would be tedious to create five different cakes with five different groups of code, so we can use a class as a template and cut our work, and amount of code, in half.

The way we create a class is by identifying the most important and fundamental aspects of an object you want to create. A class is a mold for an object, in short. We can create infinite amounts of objects from only one class, which is useful for websites that get multiple users wanting to create profiles. Twitter, Facebook, and Instagram all have so much traffic that it would be extremely difficult to individually create user profiles, so it has a template, or a class, to do it for them. 

In one line of code you can create an entire Facebook about page, simply by assigning values to an attribute of that class. This saves space, time, and energy spent on behalf of the website, making receiving traffic much easier.

For our cake example, lets say a baker wanted to code five hundred cakes. The important aspects of a cake are its width, length, shape, layers, flavor, frosting, color, and any decorations. To create a class, “Cake,” we would make a writer method to assign each of these attributes, then a reader method so that the baker could see each aspect of the cake by calling them back. If a client wanted to order a cake, it would fill in each attribute that the baker has asked for.

We also have actions to mix and bake the cake, as in real life. The difference between this method and a method to assign an attribute is that these methods actually do something to the cake, instead of just altering the look of the cake.

A disadvantage to a class can be its restrictions. There is a limited amount of variety in a class, unless it’s already coded in. For example, you can’t choose what shape the cake is unless we’ve specified that you can change/assign that attribute to your cake.

	class Cake
		def initialize(cake_flavor, width, length, color, shape, filling, number_of_layers, frosting, decorations)
			@cake_flavor = cake_flavor
			@width = width
			@length = length
			@color = color
			@shape = shape
			@filling = filling
			@number_of_layers = number_of_layers
			@frosting = frosting
			@decorations = decorations

			@decorations=[]
			@status

		end

		attr_accessor :cake_flavor, :width, :length, :color, :shape, :filling, :number_of_layers, :frosting, :decorations


		def mix_batter
			puts "batter is mixing"
			@status = "batter is mixing"
		end


		def bake (time, temperature)
				if @status == "batter is mixing"
			@time = time
			@temperature = temperature
			puts "put in for #{@time} minutes at #{@temperature} degrees"
			@status = "cake is baking at #{@temperature} degrees form #{@time} minutes"
				else puts "you need to mix the batter first!"
		end
		end

		def add_decorations (decoration)
			@decorations<<decoration
		end


	end

	Cake.new("chocolate", "5", "5", "blue", "square", "vanilla", "2", "vanilla", "candle")




http://www.tutorialspoint.com/ruby/ruby_classes.htm
http://wiseheartdesign.com/articles/2006/09/22/class-level-instance-variables/
http://www.sitepoint.com/class-variables-a-ruby-gotcha/
