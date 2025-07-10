# Design-patterns-Nutshell

## reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.
-------------------------------------------------------------------------------------------------------------------------------------------
**Adapter**

_Summary : _

A structural design pattern type that acts as a bridge  to  collaborate incompatible(different type ) interfaces

_A real world example :_

In real time ,we can relate many examples .
  -> How a micro USB charger can be used in Type c port Mobile ?
           Here Micro USB to Type C converter acts a Adaptor  

   -> How a person who knows only German  can communicate to English speaking guy ?
           Here a translator acts as an Adaptor  

_Where it can be applied ? _

  In case of existing class needs to be used with new class which has  different interface then adaptor class helps here 

_Advantages :_

  1. Reusability of existing interfaces
  2. Adaptability as per client need. Adaptor class can be modified  without modifying existing code 

_Drawbacks :_
  
  1. Increase in code size and complexity 
  2. Many adaptions in Adaptor class  might required to meet requirement

**Observer **

_Summary : _

A behavioral design pattern that helps achieve notification to all observers in case of object is modified. An object which performs notification is  publisher and objects that tracks occurrence of changes in publisher object are known as subscribers.
 
_A real world example :_

Simple example which we are using in day today life is YouTube  channel subscription.  
As stated above ,the concept of observer design pattern is whenever there is an occurrence of changes  respective subscribers needs to be notified.

In you tube channel, whenever a new video is posted ,the users who subscribed channel with notifications  gets notified Immediately . Here the YouTube channel is Publisher and all users who subscribed are subscribers. The same example applies for all SW updates ,Apps ,Etc., 

_Where it can be applied ? __

 whenever publisher needs to notify all subscribers to get the its updates  .

_Advantages :_

   1.  Instant automatic notification all  dependent objects  
   2.  Establish relations between objects at runtime.
_Drawback :__
    1.  Notification happens in random order 
    2.  Information leakage due to explicit register option for subscription 

**Mediator **

_Summary : _

The behavioral pattern which aims at avoid direct communication between objects by making them communicate through the mediator object. This  pattern reduces communication complexity between multiple objects and enables easy maintenance 

_A real world example :__

Air traffic controller is a great example of mediator pattern where the airport control room works as a mediator for communication between different flights. Mediator works as a router between objects and it can have it’s own logic to provide way of communication.

_Where it can be applied ? _

In case the system components are tightly-coupled with each other  and requires  higher maintainability  Mediator pattern can be applied which acts as a  mediator between objects for communication and reduces complexity involved. 

_Advantages :_

  1. Coupling between various components of a program can be reduced 
  2. Makes the code reusable
  3. Easier maintenance between objects
 
_Drawback :_
  1. The mediator pattern trades complexity of interaction for complexity in  
     the mediator. sometimes it may be case mediator itself hard to maintain.
     
**Proxy**

_Summary : _
 
Proxy is a structural design pattern that controls access to the original object being a substitute or alternative. This provides real functionality of another class

_A real world example :_

In day today life, lot of proxy we come across .For example ,instead of pay/withdraw amount from bank account UPI platforms Gpay or Paytm is used .Here UPI interfaces acts as a proxy.
Another example is in office ,We used to access Lab PC's via remote using virtual proxy  

_Where it can be applied ? _

Proxy pattern is used when we need to create a wrapper to cover the main object’s complexity from the client.

_Advantages :_

  1. The proxy works even if the service object isn’t ready or is not available.
  2. Ability to modify proxy without alteration of actual component/server

_Drawback :_
  1. The response from the service might be slow. Like accessing server via  
     remote PC 
