# Introduction

There is a reason you started reading this book. Fair chance that you heard about one of the buzzwords that are used to describe something which we call the Semantic Web. So let us start with them first, I am sure everyone could contribute more of them so I just start with the ones I often hear: Semantic Web, Linked Data, Web of Data, RDF, OWL, SPARQL, Graph database, Web 3.0.

Unfortunately there is a lot of confusion around those terms and the whole technology stack behind it. The idea of this book is to help interested people to bootstrap in the technology stack. I called the book Bootstrapping in the Web of Data, because that is what the technology in my opinion really is about.

## Semantic What?

Many years ago a colleague gave me and some friends an introduction to the Semantic Web. He gave a very technical presentation and explained the basic concepts, showed us some example and used a lot of terms I never heard of. I found it strange, it didn't really fit to anything I heard before and for the next few months, I forgot about it. Being an IT guy I get fed up by computers on a regular base and during that period I thought it is ridiculous that programmers create user interfaces because programmers usually suck at it. For some reason I thought that this Semantic Web thing might be worth looking at. Providing descriptions about data in the data itself was one of the things which stuck after my friends presentation. And I had the impression that this might be incredibly useful for creating smarter user interfaces by people that are not programmers but know about the data.

So I went back to my friends presentation, printed a whole bunch of W3C specifications and spend some time outside at the sun reading. I was hooked. For the first time in many years I actually thought that there is something really exciting new in the IT world. I started creating some data in a text editor and called my colleague. I wondered how the heck I can visualize this now in the web browser. Turns out this was way harder than we expected. The specifications were there but obviously there were not too many programmers caring about it yet; so it was quite hard to do something useful with it. It was 2008 and the Semantic Web was simply not there yet for average programmers and users like me.

## The Web of Data

The story of the Semantic Web is the story of the Web. Some 25 years ago Tim Berners-Lee sits at his desk at CERN in Geneva and writes a now famous proposal for an information management system. He hands it over to his boss Mike Sendall, which does not care about it for several months. Finally he gets the proposal back with a short text on it: ‘Vague, but exciting’, were the words that Sendall wrote on the proposal, allowing Berners-Lee to continue. Several years later this proposal lead to what we all know and love as The Web.

Shortly after I got interested in the Semantic Web I started reading the book Weaving the Web, where Berners-Lee explains his story of how the whole thing happened. After reading the specifications of the Semantic Web I was amazed: It became absolutely clear to me that from the beginning Tim Berners-Lee envisioned not just the Web as we know it but the Semantic Web. He just had to solve a whole lot of problems before and in the best tradition of iterative programming, he and his crew started with the basics first. So let me try to explain what the Semantic Web is based on what we know from the Web.

The Internet was there before the Web. In mid 70ies the US Department of Defense started development of something which became known as the ARPANET. This network was running on the early drafts of what we now know as the Internet protocol suite, often dubbed TCP/IP. In the early 80ies the protocols got formalized and new networks were connected to it, the Internet started to take off. There were quite some services available and the most popular ones were probably email for direct communication and newsgroups for public communication about certain topics. However, sharing documents and knowledge was not easy and there was no formalized way in doing that.

Berners-Lee came up with several fundamental ideas: Every thing we share on the web gets a unique link and we use a common way to share the content, in the Web this is a HTML document.

Now it gets a bit more complicated but in the end it boils down to this:

* The link is globally unique. Everyone can start creating links within his realm called namespace. If you for example own the domain example.org you can create unique links like www.example.org/aboutme.html.
* Documents are represented in a standardized format called HTML. In this specification Berners-Lee reused a concept he found elsewhere: Hypertext. This was the simple idea that you could point from one document to another by adding something we now know as a hyperlink.
* To make the hyperlink concept work outside of proprietary applications he also came up with a transport protocol for such documents. We all know, love and hate it under the name HyperText Transfer Protocol or short HTTP.



