# booster

Try to learn Serverless computing by building a booster bot.  

## booster bot

A booster bot accepts messages, let's say SMS, and then responds with an ego boost.

## questions

* Should there be some kind of grammar?  
* How should we get started?
* Should messages be public?
* Should it be a tweet bot instead of SMS?
  * No, SMS is more general, why get stuck on Twitter?

It seems like it should just respond to messages first.  What's the most simple booster bot?  
You send it a message, anything, and it just replies with a random message from a list of boosts.

### example

+ incoming message: *hello booster*
+ response: *you're killing it today! keep up the good work!*

The incoming messages should be saved in a database and associated with the sender.  Maybe later these can 
be used as a source of boosts.  

We could have some algorithmic mashup of boosts as a response

+ incoming: *i love palm trees*
+ response: *palm trees i love*

That's pretty simple so maybe not that interesting.  But you can see how a few tricks could end up with 
some interesting responses. So, we should also log our responses.  

What would the database schema look like?  
  + user, incoming message,timestamp
  + user, response, timestamp
  
That would allow us to reconstruct the 'conversations'.  

## What's a good minimal starting point?

Just accept a message and send back 'hello'.




  
  
