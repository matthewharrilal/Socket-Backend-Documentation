#### THE REASONING!

##### Utilizing socket.io for forms of communication that help in ways the HTTP protocol can not. What I mean by that is for a group chat application there is a certain dynamic in how you recieve messages. If we think in terms of the standard HTTP protocol everytime we want to send a message from one user to another we would have execute a network request. If you have ever been in a group chat you know how easy it is for dozens of messages to be sent at once!

#### Current Solutions!

##### Well ... there is something that can kinda ... sorta ... well actually there is HTTP long polling, and what that is everytime the server sends back a response we can send another request to constantly check if there is more subsequent information. This acts independently of a client induced request. Acts like someone who keeps falling asleep they wake up and they're alert for a period of time but then they sleep ... or in this case the connection is closed!


#### What are web sockets?

###### Well web sockets act as an open pipeline between the server and the client. This can be visualized as  a plastic tube. Information or data can be sent bi-directionally through this tube(pipeline). This connection remains open continuously until one side of the connection is closed ... or in this case someone covers the other side of that darn tube! With this network requests that are sent don't automatically close the connection after processed and responded to instead that connection remains open just waiting for requests to come through! 
