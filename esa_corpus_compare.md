% What shall we talk about at ESA?
% Noam Ross
% 14-07-17 20:49:15



[ESA](http://esa.org/am/) is just around the corner, and many of us are gearing
up and trying to figure out a [schedule](http://eco.confex.com/eco/2014/schedule/index.cgi)
to cover all the topics that interest.  ESA is a big conference and there's far
too much for any one person to see.  In the end, everyone experiences a [different part of the elephant](http://en.wikipedia.org/wiki/Blind_men_and_an_elephant).  I thought it would be interesting to take a look at the big picture, though,
and examine the ESA program as a  *whole* to see what could be learned.  This
is the first of (maybe) several posts where I use some basic text-mining tools
to explore the content of the ESA program.




First, what are the most common terms in the ESA program?






![](figure/plot1.png) 

Few surprises here.  "Species" would have been my guess for the top.  "Plants"
are probably on top because ecologists usually refer to animals by various
sub-groups.  The rest are fairly ho-hum: ecology and science-y words.

A much more interesting question is, how do the topics at ESA change from year
to year? Below I show the terms that changed whose use in ESA abstracts changed 
the most between 2013 to 2014:

![](figure/mung.png) 

This paints a much more interesting picture.  The rise of California
and the fall of Minnesota make sense given the change in the meeting's location.
But we can see the influence of landscape on topics as well.  We see fewer
words associated with freshwater ecosystems, prairies, and forests this year,
and more associated with fire and other plant systems. Also, we see a difference
in the *kinds* of ecology in the program. This year there are fewer words
like *biomass* and *nutrient* - those common in ecosystem ecology - and more
like *pollinator*[^1], *phenology*, and *network* - those associated with
the study of species interactions.

[^1]: "pollinia" is a stand-in for all pollination-related words here, as I
applied [stemming](http://en.wikipedia.org/wiki/Stemming) to the txt.

These are the biggest *changes*, but have the *big themes* changed?  The plot
below is similar, but instead of plotting the words with the greatest absolute
change, I plot the relative change of 50 words most common across both years:

![](figure/big.png) 

Many of the patterns are the same here: "California" still comes out on top and
"biomass" on bottom.  But a few other interesting things stand out.  Management-related
words - "use", "conserve", "risk" - are always popular but more prevelant this year,
as are geographic terms like "island" and "landscape".

It's possible that these changes are due to changes in what's popular in ecology,
but it is likely that much of the concepts captured in these terms - ecosystem,
community, and landscape ecology - are influenced by region, as well.  After all
an ecosystem perspective is likely to dominate in the midwest, where an abundance
of lakes have been important in the research of freshwater nutrient cycling,
and a landscape perspective may be important in California, which has such
heterogeneity of habitats.  This is a pretty good argument for keeping ESA's
location moving year-to-year, so that no regional perspective dominates every
year.

That's just a quick first pass.  Check out [this repository on github]() for the
code that generated these plots and how to grab the ESA program text for your
own use.  See you in a few weeks!