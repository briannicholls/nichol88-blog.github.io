---
layout: post
title:      "Object Lifecycle in Ruby"
date:       2020-03-24 16:36:04 +0000
permalink:  object_lifecycle_in_ruby
---


I was inspired to write this post when seeing the prompt from Flatiron, 'Write about how you handle object lifecycle'. But, we learn Ruby, and I don't even have to think about object lifecycle! But I was inspired to learn more, since I aspire to delve into other languages, and want to learn as much as possible.

'Object Lifecycle' refers to the creation and destruction of an object. More specifically, it refers to how memory is allocated and deallocated to and from that object. In Ruby, this is all handled behind the scenes quite intelligently. How a particular language handles this is commonly referred to as "garbage collection". While my understanding is still limited on the subject, in Ruby, memory is deallocated from an when there are no more references to that object. Which is pretty cool. I came across a unique Ruby module that will allow you to interact with some of these background processes, called ObjectSpace. You can use ObjectSpace to see what objects are currently in memory (the "heap"), and see when objects are destroyed and when the memory is deallocated. There is also the GC module (Garbace Collector), which allows you to interact with the garbage collector deirectly, for example to disable it completely with `GC.disable`.

It's all above my head, but they are new modules I didn't know about before, and they are essential to the language, so it's interesting to learn about. I have always wondered what goes on behind the scenes, as Ruby isn't necessarily considered a 'fast' language compared to others, because it favors ease of use. I assume this is one of those things. I definitely don't want to have to manage objects lifecycle - I would rather focus on coding! That being said, evaluating how memory is managed using these modules would be a useful skill, especially in larger applications. Writing a program that can see potential issues might be something few are doing, and I will definitely consider delving deeper in the future.
