# Redis-Pub-Sub

This code is to demonstrate what PubSub is, and to visualize how it works.

# What is Redis PubSub?
Firstly, PubSub stands for Publish and Subscribe. So, one person will be publishing and the other will bbe subscribing.

Imagine you are running a radio channel, say 91.1 FM. You are PUBLISHING your music shows in that channel. 
A person, say B is tuning his radio receiver to 91.1 FM. So he is SUBSCRIBING to your channel.

Redis PubSub works in the same way as well.

Inorder to visusalize this concept, open your Redis-CLI and give the following command:
      PUBLISH fmshow
      
You would get the output to be 0.
This is because no one has subscribed to the channel you have created right now.

So, to subcribe, open another redis cli and enter the following command:
      SUBSCRIBE fmshow
Now, come back to your first cli, you would have got your first subscriber!

# Code
The code is to visualize how PubSub is implemented in Python.
In redis_publisher.ipynb, a json data is published in a redis channel.
In redis_subscriber.ipynb, we subscribe to the redis channel in order to fetch the json data published in that particular channel.



 
