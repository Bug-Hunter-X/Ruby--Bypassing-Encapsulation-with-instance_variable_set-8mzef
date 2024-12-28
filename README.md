# Ruby: Bypassing Encapsulation with instance_variable_set

This example demonstrates a potential pitfall in Ruby: directly modifying instance variables using `instance_variable_set`.  While sometimes useful for metaprogramming, it can easily lead to unintended consequences, breaking encapsulation and making code less maintainable.

The `bug.rb` file shows how `instance_variable_set` bypasses the normal getter method, making changes outside the defined interface of the class.

The `bugSolution.rb` file offers a better solution using a setter method.