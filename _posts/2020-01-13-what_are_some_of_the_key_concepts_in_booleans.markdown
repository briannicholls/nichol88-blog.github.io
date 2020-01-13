---
layout: post
title:      "What are some of the key concepts in Booleans?"
date:       2020-01-13 14:41:47 +0000
permalink:  what_are_some_of_the_key_concepts_in_booleans
---


Booleans are a Data type with only two possible values - True, or False. However, other data types can be considered 'truthy' or 'falsey'. For example, 'nil' or '0' would be considered 'falsey'. So if you have a function that returns a falsey value, it would evaluate to the Boolean 'false'. This is helpful for adding checks to your code, to make sure a function is working properly, or to handle it appropriately if it is not.


```
def shorter_than_5?(string)
    if string.length < 5
		   string
		else
		   nil
		end
end
```

Here is a function that accepts a string, and if the string has a .length greater than 5, it will return that string, otherwise returning 'nil'. While this function does not explicitly specify and Booleans, we can still use the concept of Booleans to check our code and handle it appropriately. For example:

```
if shorter_than_5?('cat')
   puts "This will print"
end

if shorter_than_5?('elephant')
   puts "This will not print"
end

```

In the first 'if' statement, we use the 'shorter_than_5?' function. Notice that even though the value returned by the function is a string, it is considered 'truthy' and the if statement evaluates it as if it were equal to 'true'. Likewise, in the second 'if' statement, the string 'elephant' will cause our function to return 'nil', a 'falsey' calue, and our 'puts' will not print.

Using 'Falsey' and 'Truthy' and understanding how your language interperets them is necessary to write effective code. The concept of a binary piece of data is present at the lowest level of machine code, i.e. 'ones and zeros'. So with Booleans, you're speaking the computer's language!
