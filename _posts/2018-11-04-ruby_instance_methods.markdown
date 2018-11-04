---
layout: post
title:      "Ruby Instance Methods"
date:       2018-11-04 22:31:11 +0000
permalink:  ruby_instance_methods
---


Class vs. Instance Methods 

Class methods are methods that are called on a class and instance methods are methods that are called on an instance of a class. 

class Foo
    def self.bar
       puts 'class method'
  end
  
  def baz
      puts 'instance method'
    end
end

Foo.bar # => "class method"
Foo.baz # => NoMethodError: 

Foo.new.baz # => instance method
Foo.new.bar # => NoMethodError: 

The key difference between class and instance methods is instance methods only work with an instance and thus you have to create a new instance to use them (Foo.new). 

