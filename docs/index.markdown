---
layout: default
---
![Homepage Banner](/assets/images/kleinbottlebanner.png){:width="90%"}

{% include linkedHeading.html heading="introduction" text="introduction" level=1 %}
This site is part of my final project for the first semester of Mrs. Reyes's multivariable calculus course! It's hosted by GitHub Pages at [this repository](https://github.com/nmokey/klein-bottle){:target="_blank"}{:rel="noopener noreferrer"}, and is built with Jekyll and written in Markdown. 

For my project, I'm focusing on exploring a specific subset of topological spaces called **non-orientable manifolds**, their definitions and fascinating properties, and their connection to multivariable calculus. Topology has a lot of jargon, so I will quickly go over some basic definitions so everything is relatively easy to understand, but it probably means that I'll be making some simplifications and saying things that are only *technically* right. In addition to drawing connections between Klein bottles and multivariable calculus, I'll also discuss other non-orientable manifolds and topology topics. 

{% include linkedHeading.html heading="artwork" text = "artwork" level=1 %}
Work in progress.

{% include linkedHeading.html heading = "orientability" text="what is orientability, anyway?" level=1 %}
To understand **non-orientable manifolds**, we can break the term into two pieces: defining *orientability* and defining *manifolds*. (Unfortunately this strategy doesn't mecessarily work for all math concepts, like "*hairy ball theorem*" and "*space curve*.")

In topology, a **manifold** is a topological space which locally resembles Euclidean space near each point. Surfaces are simply 2-dimensional manifolds, so when we talk about non-orientable surfaces for all intents and purposes they're basically the same thing. An $n$-manifold is simply a thing that lives in $n$-dimensional Euclidian space (it's more nuanced than this, but it's close enough).   

![orientable surfaces](/assets/images/orientable.png){:width="80%"}

There are a couple ways to think of **orientability**: the formal definition is that it's a property of topological manifolds which permits a consistent sense of clockwise and counterclockwise. If you choose a direction of a normal vector and keep assigning normals along the surface, when you loop back around to your starting point the normal vector should still point in the same direction.  

*Side note: orientability is also a concept for curves. **Curve orientation** is simply the choice of which direction you travel along the curve. For example, the x-axis pointing right and y-axis pointing up are technically orientations. Closed curves can either be positively/counterclockwise oriented or negatively/clockwise oriented.*

In popular mathematics, a surface that's **non-orientable** is usually described as having only one side, partially because that's the most exciting way to put it. You can imagine an ant walking along the surface of a Klein bottle: starting on the "outside", the ant can crawl through the tube and onto the opposite side of its starting point without ever crossing a boundary or edge, which means that the surface only has one side, and no "inside" or "outside." That's pretty neat! The formal definition is basically the opposite of orientability: it's a property of a surface where you can't consistently define clockwise and counterclockwise.  

On a non-orientable surface, you can't integrate vector fields (e.g. surface integrals, line integrals) because you can't reconcile the inconsistent surface normals. You can still take multiple integrals and things like that, to find volumes.

{% include linkedHeading.html heading = "klein bottle" text="the one and only klein bottle" level=1 %}
Named after [Felix Klein](https://en.wikipedia.org/wiki/Felix_Klein){:target="_blank"}{:rel="noopener noreferrer"}, who imagined it in 1882 (linked in case you want to make fun of his picture).  

Constructing a Klein bottle is simple. Take an open cylinder, extend one end of it and bend it around to go back through itself, and smoothly connect the ends. Did you follow along? Awesome! You now have your very own Klein bottle.  
![anatomy](/assets/images/anatomy.png){:width="90%"}

Let's do a quick rundown of some amusing, fascinating facts about Klein bottles:
- one side
- zero volume (perfect for alcohol), since it does not doesn't separate the universe into two parts
- 4d manifold immersed in 3 dimensions for us lowly humans to observe (see below)
- composed of two mirror-image möbius strips glued together
- pretty easy to fill, almost impossible to empty
- Y2K compliant ✓
- Euler characteristic of 0, given by vertices - edges + faces
- genus of 1, loosely meaning it has one hole

Ok, so we understand what a Klein bottle is conceptually. The nice thing about topology is that it doesn't matter how we bend or stretch our surfaces, they still retain the same properties. But what if we wanted to take a look at some equations that can give us an idea of what "version" of a Klein bottle we're actually seeing?

This is where the multivariable calculus comes in. Clifford Stoll, topologist and purveyor of [fine glass Klein bottles](https://www.kleinbottle.com/){:target="_blank"}{:rel="noopener noreferrer"}, offers the [following parametrization](https://www.desmos.com/3d/a0c3f74c53){:target="_blank"}{:rel="noopener noreferrer"} of a Klein bottle as an alternative to buying one:  

$$x(u,v) = \cos(u)\cos(\frac{u}{2})(\sqrt{2}+\cos(v))+\sin(\frac{u}{2})\sin(v)\cos(v)$$  

$$y(u,v) = \sin(u)\cos(\frac{u}{2})(\sqrt{2}+\cos(v))+\sin(\frac{u}{2})\sin(v)\cos(v)$$  

$$z(u,v) = -\sin(\frac{u}{2})(\sqrt{2}+\cos(v))+\cos(\frac{u}{2})\sin(v)\cos(v)$$  

It's important to note that Klein bottles are 4d manifolds immersed in 3d space so we can visualize them: in their "true form," they have no self-intersection (also called a nexus). But here's an idea: what if I wanted to break my brain and consider parametrizations of 4d Klein bottles and their 3d embedded counterparts to try to get a glimpse of what Klein Bottles *should* look like? Of course, since this parametrization has 3 variables, it represents an **immersion** of the manifold in $\mathbb{R}^3$ space. All the Klein bottles that we're able to see and visualize are immersions in 3d space. A *true* Klein bottle needs 4 dimensions so that it Besides this one, there are two other common immersions of the manifold: the left-handed and right-handed figure-8 immersions, which are *chiral*.

You might notice the parametric equations above are functions of $u$ and $v$ rather than $x$ and $y$: this indicates a **change in variables**, meaning we've taken the domain of some function and transformed it into another coordinate system that makes the domain of that function much nicer to look at. 

{% include linkedHeading.html heading = "examples" text="other examples of non-orientable manifolds" level=1 %}
## möbius strip
Named after [August Ferdinand Möbius](https://en.wikipedia.org/wiki/August_Ferdinand_Möbius){:target="_blank"}{:rel="noopener noreferrer"}, who discovered it as a mathematical object in 1858, although the shape appeared as early as the 3rd century in Roman mosaics.  

The Möbius strip is probably the most well-known non-orientable surface, since it's much easier to implement in architecture and whatnot than Klein bottles. Möbius strips are essentially Klein bottles 1 dimension down: if you cut a Klein bottle in half (if for some reason you'd deface such a beautiful surface), you'd get two mirror-image Möbius strips: a left-handed one and a right-handed one. You can easily make one yourself by taking a strip of paper, half-twisting it, and gluing the ends together. In differential gemoetry, you construct one by taking the space swept out by a line segment rotating in a plane that is also rotating. This is given by the [following parametrization](https://www.desmos.com/3d/ebeac4bd6e){:target="_blank"}{:rel="noopener noreferrer"}:

$$x(u,v) = (1+\frac{v}{2}\cos{\frac{u}{2}})\cos{u}$$

$$y(u,v) = (1+\frac{v}{2}\cos{\frac{u}{2}})\sin{u}$$

$$z(u,v) = \frac{v}{2}\sin{\frac{u}{2}}$$

for $0 \le u \le 2\pi$ and $-1\le v \le 1$, where $u$ is the rotation angle of the plane and $v$ is the position of a point along the rotating line segment.
## roman surface

## real projective planes
A Möbius strip is a punctured projective plane, and since a Klein bottle is two Möbius strips glued together, it follows that a Klein bottle is the connected sum of 2 real projective planes.

{% include linkedHeading.html heading="applications" text="\"applications\" of non-orientable manifolds" level=1 %}
Since topology is a field so deep in pure mathematics, it's hard to find actually useful applications of a topic so niche and abstract as non-orientable surfaces, so I'm stretching the meaning of "applications" a little bit to include anywhere non-orinetable surfaces pop up in real life, not necessarily applied in any useful way.

Due to their highly recognizable form, Möbius strips in particular have become popular in graphic design and architecture, but there are also some practical uses. Here's a list:
- google drive logo
- recycling symbol
- cutting bagels
- bacon loops
- pasta (goes well with fractal broccoli)
- scarves and hats
- mobius bench
- industrial belts (to wear evenly on "both" sides)
- mobius resistors
- bach's 5th canon

{% include linkedHeading.html heading="why" text="what's the point?" level=1 %}
There are certain topics that are so intrinsically fascinating that you can’t rest until you find out more. The only way I can describe it is the sort of feeling that you get when you learn for the first time that a Mobius strip - or in my case, a Klein bottle - is nonorientable, essentially meaning that it has only one side (a pretty high level explanation). You sort of think to yourself well, that doesn’t sound right. You look at one and start tracing it in the air with your finger, slowly realizing *holy crap, this thing actually does only have one side… how? why?*  

I think that this sense of awe is universal and everyone has their own topics that elicit that feeling. For me, Klein bottles and the whole concept of non-orientability have been a continuous fascination. so I’m excited for the opportunity to share why I think it’s interesting. Nonorientable surfaces in particular are relatively far from applied math, and so my why for choosing to explore them in further depth does not lie in any sort of external use but rather that intrinsic curiosity.  

*This explanation for why I care about Klein bottles was copy-pasted verbatim from my project proposal.*  

{% include linkedHeading.html heading="references" text="references" level=1 %}
Alling, Norman, and Newcomb Greenleaf. “Klein Surfaces and Real Algebraic Function Fields.” *Bulletin of the American  
&emsp;&emsp;&emsp;&emsp;Mathematical Society*, vol. 75, no. 2, 21 Feb. 1969, pp. 869–872, https://doi.org/10.1090/bull/1969-75-02. 

Ferréol, Robert. “Klein Bottle.” *Klein Bottle*, 2017, mathcurve.com/surfaces.gb/klein/klein.shtml. 

Munroe, Marshall Evans. “Multiple Integrals - Oriented Manifolds.” *Modern Multidimensional Calculus*, Reprint ed.,  
&emsp;&emsp;&emsp;&emsp;Dover Publications, Inc, Mineola, New York, 2019, pp. 263–268. 

Stoll, Clifford. “What Is a Klein Bottle?” *What Is a Klein Bottle?*, Acme Klein Bottle, Dec. 2021,  
&emsp;&emsp;&emsp;&emsp;www.kleinbottle.com/whats_a_klein_bottle.htm. 

Lots of Wikipedia