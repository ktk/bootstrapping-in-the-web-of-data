We often get asked where to start with Semantic Web and RDF. There are probably many ways to do this and on this page you will find the one I found useful for myself. There is a lot of stuff to read so let us start
with some basics first:

* [RDF Primer](http://www.w3.org/TR/rdf-primer/) - This is a excellent introduction to RDF and the general concepts of the Semantic Web. Start here!
-   RDF can be serialized in many ways. If you start creating your first triples in a text editor you want to use [Turtle](http://www.w3.org/TeamSubmission/turtle/) serialization. If you are a programmer you might want to have a look at [RDF/JSON](http://docs.api.talis.com/platform-api/output-types/rdf-json) and [JSON-LD](http://json-ld.org/). The most popular one is probably [RDF/XML](http://www.w3.org/TR/rdf-syntax-grammar/) but let your computer serialize that for you :) Don't worry too much about that right now. If you can read Turtle you are ready for a good start.

Then it is time to do some hands-on stuff. I recommend to create a
[FOAF](http://en.wikipedia.org/wiki/FOAF_%28software%29) representation
of yourself. Check some examples to get some hints:
[me](http://ktk.netlabs.org/foaf.rdf) (Adrian),
[Bart](http://bart.netage.nl/foaf.rdf) and
[Christian](http://www.clanganke.de/foaf.rdf). [Tim
Berners-Lee](http://www.w3.org/People/Berners-Lee/card) has a more
advanced but also more complex one. You might want to create this with
some [help](http://www.ldodds.com/foaf/foaf-a-matic) first and then
adjust it according to the [FOAF
specification](http://xmlns.com/foaf/spec/). You might have noticed that
our profiles are using RDF/XML serialization, which is not very easy to
read. So let us transform that into something else: Install
[Rapper](http://librdf.org/raptor/rapper.html) on your system and
convert the profile into Turtle. Use
[wget](http://en.wikipedia.org/wiki/Wget) or
[curl](http://en.wikipedia.org/wiki/CURL) to get my profile (assuming
you are on MacOS/Unix):

    curl -O http://ktk.netlabs.org/foaf.rdf

followed by a conversion from RDF/XML to Turtle:

    rapper -i rdfxml -o turtle foaf.rdf > ktk.turtle

ktk.turtle now contains my FOAF profile in Turtle syntax. If you now
install [Graphviz](http://www.graphviz.org/) as well you will also get a
binary called [dot](http://en.wikipedia.org/wiki/DOT_language) on your
system. So try this:

    rapper -i rdfxml -o dot foaf.rdf | dot -Tpdf -oktk.pdf

If you open ktk.pdf you should see a nice graph of my profile. If you
then do that for your own FOAF profile you just bootstrapped your very
own part of the Semantic Web. Congratulations! It is now a good moment
to upload your own file to your website, like we did with ours. Try to
use a URI which stays there for as long as possible. Now let us finish
this introduction with some more reading:

-   The current web consists mostly of HTML documents. To add the
    expressiveness of RDF to HTML (or any other XML format) we can use
    [RDFa](http://en.wikipedia.org/wiki/RDFa) which is specified at
    [W3](http://www.w3.org/TR/rdfa-syntax/) as well.
-   As you can imagine your FOAF profile is one among billions of other
    pieces of information out there in the Semantic Web. The [Linked
    Data Tutorial](http://ld2sd.deri.org/lod-ng-tutorial/) gives some
    more ideas about what you have to consider if you want to do that on
    a large scale.
-   If you have some more time you should read the book written by one
    of the authors of the Linked Data Tutorial called [Linked Data:
    Evolving the Web into a Global Data
    Space](http://linkeddatabook.com/editions/1.0/).
-   And last but not least check out the [Linked Open Data (LOD) cloud
    diagram](http://richard.cyganiak.de/2007/10/lod/) (updated around
    once a year) and check how it evolved over the past few years (
    [2007](http://richard.cyganiak.de/2007/10/lod/lod-datasets_2007-11-07.png),
    [2008](http://richard.cyganiak.de/2007/10/lod/lod-datasets_2008-09-18.png),
    [2009](http://richard.cyganiak.de/2007/10/lod/lod-datasets_2009-07-14.png),
    [2010](http://richard.cyganiak.de/2007/10/lod/lod-datasets_2010-09-22.png)).
    Pretty impressive, right?

