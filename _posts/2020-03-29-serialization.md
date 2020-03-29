---
layout: post
title: "Serialization"
categories: [java, programming]
---

The first time I saw a class implementing a Serializable interface, I was like, okaaay, so what is this? Why do some class implement this while others don’t?

{% highlight java %}
public class Employee implements Serializable
{% endhighlight %}

### What is the Serializable interface in Java?
In Java, this interface is used as a marker for your class if you want to make your object serializable. If you check this interface out, you’ll see that it doesn’t have any implementation.

In programming, serialization is the process of transforming the structure of a data into a serialized form. It is transformed in a form of byte stream that can be saved in a file or transported over a network.

### Why would you serialize your data?

We serialize our data if we transfer them from one place to another, e.g. from one application to another application. In the case of objects, because they have a life cycle and they only live within the lifetime of our program, it’s just not possible to send them out in their current structure. This is where serialization comes into play. We want a mechanism to save the state of our object or the data that our object currently holds into a series of bits before sending it over the network. The receiving end can then transform the bits back into its original form, this is called deserialization.

This is obviously just a simplified explanation of the process, but this is how it works in general, and this is why this concept exists in the computing world.
