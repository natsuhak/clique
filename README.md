# Clique

## Objective

Our objective is to democratize social media, and treat it as the tool it should be. 

Currently a work in progress, Clique is designed to be a open-source environment for self-hosted social media, allowing groups of people to
host their own instant messaging services, photo sharing spaces, professional and dating networks and much more.

### Why?

The main reason we decided to begin this project is to have control over our personal lives. Contact with our family and friends has never been 
easier than it is today, however the apps and platforms that provide it are for profit enterprises that don't always take personal wellbeing
into account.

What if we were able to control how our communication channels work? What if our apps didn't treat our attention as an economic asset?
What if we escape the seemingly inevitable ad-based monetization model? What if social media was built by all the people that use it?

### So you guys want to be the next billion dollar company?

Nope. Clique is designed to be a tool, not a company, not a service. Actually... is planned to be a **set of tools** that
everyone can use, manage or modify as they see fit.

### What makes it different to every other open source project?

Nothing really.

### Where will the money to make it work come from?

You have to pay for yourself of course.

### Y tho?

It wouldn't be sustainable in any other way. Think about Clique like you think about your house: you definitely didn't got it for free, you have to pay
the bills to keep the lights on and, if the neighbors hear you doing weird stuff, the police will bang on your door.

### What's the benefit then?

Just like your house, it is a place where you can hang out with family and friends, a place you can control as you like and a collaborative
effort where everyone that benefits can share the cost.

## How will you do it?

Have you seen all those services to build personal websites? Well, the plan is to do the same thing for social media platforms. 

If you want to communicate or share content with your family and friends without a third party selling your data, you set up your own platform.
This means that you will cover hosting and domain costs, but all the **tools** will be there to make it as easy and painless as possible. If it
seems that covering the cost for an entire year by yourself is too much, you can always ask your friends to help 😉. 

This comes with a lot of caveats though (here we mention a few):

* Multiple personal platforms running different code would be a mess, should people install a different app for every Clique server they want to
participate in?
* Each person using someone else's Clique server has to trust the adminstrator, wouldn't this allow malicious actors to take advantage of other people?
* What happens if the administrator doesn't pay and the server goes down?
* Who is responsible for the content inside the server?
* How variable would be the performance between different clique servers?

To address these problems we propose to build Clique in layers with a very rough roadmap:

### Security Layer and IM Client

This is the heart of Clique

* Design a core security layer that every Clique server should follow. Allowing end-to-end encrypted communication between any two members of the Clique server.
* Create a minimal IM Clique server template that satisfies the requirements of the security layer for Instant Messaging.
* Build a standard client (web/mobile) to interact with the IM Clique server, the client should be able to verify that the server complies with the requirements of the security layer.
* Write a first version of the deployment tutorial for non-tech people to go from zero to a self hosted IM Clique server.

### Social Layer

Given that resources are limited, each Clique server should contain a few selected members (your Clique). And, instead of scaling vertically, Clique servers would be decentralized
and scale horizontally. Such infraestructure allows the same person to participate in two or more Cliques that contain different groups of people and managed by different administrators.

* Design a social layer that provides both administrators and members the capability to invite new members into the Clique, 
  establish content permissions between members inside the Clique, content moderation and member removal.
* Create a mminimal Socal Clique server template that incorporates functionality defined in the social layer.
* Integrate social capabilities into the standard client
* Update the deployment tutorial to go from zero to a self hoste Social Clique server.

### Media Layer

Why stop at messaging? Let's add what we like the most from social media, gotta share those spicy memes.

* Add image and video capabilities to IM and Social Clique servers. Images in chat, member profiles, etc.
* Add image and video compatibilty in the standard client
* VoIP? Video Chat?

### Status Layer

It should be easy for the members of the Clique to know what is happening, check on server status and help cover costs.

* Build status dashboard that provides performance metrics, days until domain and hosting expiration
* Establish pooling mechanisms for the members to finance Clique upkeep and improvements.

### Deployment Layer

The main objective is to democratize social media, so we want everyone to be able to deploy a Clique server, and the process to be as easy as buying a product online.

* Incorporate the main steps of the deployment tutorial into the standard client, such that members are able to select preset hosting instances, pay them and install 
  Clique server code in one day.

## Who will do it?

This is no trivial project, so we expect all the community to participate. If you want to contribute, the help is greatly appreciated.

Clique should be a platform truly made by the people for the people, so if you think there is stuff that the proposed roadmap is missing or that is non-essential, let us know!


