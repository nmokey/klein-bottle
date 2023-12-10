---
layout: default
---
![Homepage Banner](/assets/images/kleinbottlebanner.png){:width="90%"}

{% include linkedHeading.html heading="introduction" text="introduction" level=1 %}
This site is part of my final project for the first semester of Mrs. Reyes's multivariable calculus course! It's hosted by GitHub Pages at [this repository](https://github.com/nmokey/klein-bottle){:target="_blank"}{:rel="noopener noreferrer"}, and is built with Jekyll and written in Markdown. 

For my project, I'm focusing on exploring a specific subset of topological spaces called **non-orientable manifolds**, their definitions and fascinating properties, and their connection to multivariable calculus.  

{% include linkedHeading.html heading="artwork" text = "artwork" level=1 %}
Work in progress.

{% include linkedHeading.html heading = "orientability" text="what is orientability, anyway?" level=1 %}
To understand *non-orientable manifolds*, we can break the term into two pieces: defining orientability and defining manifolds. 

In topology, a **manifold** is a topological space which that locally resembles Euclidean space near each point. Surfaces are simply 2-dimensional manifolds, so when we talk about non-orientable surfaces for all intents and purposes they're basically the same thing.  

There are a couple ways to think of **orientability**: the formal definition is that it's a property of topological manifolds which permits a consistent sense of clockwise and counterclockwise. If you choose a direction of a normal vector and keep assigning normals along the surface, when you loop back around to your starting point the normal vector should still point in the same direction. 

In popular mathematics, a surface that's **non-orientable** is usually described as having only one side, partially because that's the most exciting way to put it. You can imagine an ant walking along the surface of a Klein bottle: starting on the "outside", the ant can crawl through the tube and onto the opposite side of its starting point without ever crossing a boundary or edge, which means that the surface only has one side, and no "inside" or "outside." That's pretty neat! The formal definition is basically the opposite of orientability: it's a property of a surface where you can't consistently define clockwise and counterclockwise. 

{% include linkedHeading.html heading = "klein bottle" text="the one and only klein bottle" level=1 %}
Named after [Felix Klein](https://en.wikipedia.org/wiki/Felix_Klein){:target="_blank"}{:rel="noopener noreferrer"} (linked in case you want to make fun of his picture).  

Constructing a Klein bottle is simple. Take an open cylinder, extend one end of it and bend it around to go back through itself, and smoothly connect the ends. Did you follow along? Awesome! You now have your very own Klein bottle.  
![anatomy](/assets/images/anatomy.png){:width="90%"}

Let's list some amusing, fascinating facts about them:
- only one side
- zero volume (perfect for alcohol)
- actually 4d manifolds immersed in 3d
- composed of two (mirror image) möbius strips glued together
- Euler characteristic of 0
- genus of 1

Ok, so we understand what a Klein bottle is conceptually. It's important to note that klein bottles are 4d manifolds immersed in 3d space so we can visualize them: in their "true form," they have no self-intersection (also called a nexus). But here's an idea: what if I wanted to break my brain and use level surfaces to project them into 3d space and try to get a glimpse of what Klein Bottles *should* look like?  

This is where the multivariable calculus comes in. Clifford Stoll, purveyor of [fine glass Klein bottles](https://www.kleinbottle.com/){:target="_blank"}{:rel="noopener noreferrer"}, offers the following parametrization of a Klein bottle as an alternative to buying one:  

$$x = \cos(u)\cos(\frac{u}{2})(\sqrt{2}+\cos(v))+\sin(\frac{u}{2})\sin(v)\cos(v)$$  

$$y = \sin(u)\cos(\frac{u}{2})(\sqrt{2}+\cos(v))+\sin(\frac{u}{2})\sin(v)\cos(v)$$  

$$z = -\sin(\frac{u}{2})(\sqrt{2}+\cos(v))+\cos(\frac{u}{2})\sin(v)\cos(v)$$  

Of course, since this parametrization has 3 variables, it represents an immersion in $R^3$ space. There are other ways to represent an immersion, like

{% include linkedHeading.html heading = "examples" text="other examples of non-orientable manifolds" level=1 %}
## möbius strip
Named after [August Ferdinand Möbius](https://en.wikipedia.org/wiki/August_Ferdinand_Möbius){:target="_blank"}{:rel="noopener noreferrer"}.  

Mobius strips are essentially the 
## roman surface

## real projective planes
A Mobius strip is a punctured projective plane, and since a Klein bottle is two Mobius strips glued together, it follows that a Klein bottle is the connected sum of 2 real projective planes.

{% include linkedHeading.html heading="applications" text="applications of non-orientable manifolds" level=1 %}
Since topology is a field so deep in pure mathetmatics, it's hard to find actually useful applications of a topic so niche and abstract as non-orientable surfaces, so I'm stretching the meaning of "applications" a little bit to include anywhere non-orinetable surfaces pop up in real life, not necessarily applied in any useful way.
- google drive logo
- recycling symbol
- cutting bagels
- bacon loops
- pasta (goes well with fractal broccoli)
- scarves and hats
- mobius bench
- industrial belts
- mobius resistors
- bach's 5th canon

{% include linkedHeading.html heading="why" text="what's the point?" level=1 %}
There are certain topics that are so intrinsically fascinating that you can’t rest until you find out more. The only way I can describe it is the sort of feeling that you get when you learn for the first time that a Mobius strip - or in my case, a Klein bottle - is nonorientable, essentially meaning that it has only one side (a pretty high level explanation). You sort of think to yourself well, that doesn’t sound right. You look at one and start tracing it in the air with your finger, slowly realizing *holy crap, this thing actually does only have one side… how? why?*  

I think that this sense of awe is universal and everyone has their own topics that elicit that feeling. For me, Klein bottles and the whole concept of non-orientability have been a continuous fascination. so I’m excited for the opportunity to share why I think it’s interesting. Nonorientable surfaces in particular are relatively far from applied math, and so my why for choosing to explore them in further depth does not lie in any sort of external use but rather that intrinsic curiosity.  

*This explanation for why I care about Klein bottles was copy-pasted verbatim from my project proposal.*  

{% include linkedHeading.html heading="references" text="references" level=1 %}
Ferréol, Robert. “Klein Bottle.” *Klein Bottle*, 2017, mathcurve.com/surfaces.gb/klein/klein.shtml. 

Stoll, Clifford. “What Is a Klein Bottle?” *What Is a Klein Bottle?*, Acme Klein Bottle, Dec. 2021, www.kleinbottle.com/whats_a_klein_bottle.htm. 

Lots of Wikipedia