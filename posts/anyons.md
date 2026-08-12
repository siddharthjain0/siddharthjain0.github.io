Physicists always try to break down the universe to its smallest constituents
and see what everything's made up of. We don't like to sound clueless about
things and consider it our responsibility to explain the workings of the
universe to muggles (other people). So, even if we are not sure about
something, we try our best to make a story around it and invent some cool
maths to support the story and convince people that we are smart. There are
many stories (theories) that we have invented to demystify the world.

Earlier we used to believe that everything is made of particles and there are
4 fundamental forces acting between those particles, holding them, that build
up everything. Then, one of the most successful physical theories of all time,
quantum field theory, came which told us that there are fields pervading the
universe and particles are nothing but ripples in those fields. Although,
fundamentally this is the case, in many cases we don't need full field theory.
It serves us well to consider particles and forget about fields. What we are
going to talk about is what kind of particles are possible in our world.

> A particle is a unitary irreducible representation of the Poincaré group.

In QM, we impose exchange properties of identical particles in an ad hoc way by
symmetrizing or anti-symmetrizing the wave function. It doesn't really tell us
how that comes about, and also ignores the possibility of a wave function that
is in between the two.

## Leinaas and Myrheim

We will construct the possibility of anyons starting from classical mechanics.

## Connectedness

A manifold is simply connected (or 1-connected) if for any two points on it,
all paths connecting those two can be deformed to other without leaving the
manifold during the deformation. There is one equivalence class of paths for
any two points. Any closed loop can be shrunk to a point without leaving the
manifold.

It is doubly connected (2-connected) if there are two equivalence classes of
paths connecting two points. Those two cannot be deformed to each other
without leaving the manifold. This implies there is some kind of hole
(puncture) in the manifold. The hollow inside a hollow sphere is not a hole we
are talking about. More precisely, we mean a "handle" such as in a torus.

Infinitely connected means infinite equivalence classes of paths (or closed
loops). A surface with infinite holes. A circle is an example of this.

A hole in $X$ is, informally, a thing that prevents some suitably-placed sphere
from continuously shrinking to a point. $X$ is called $n$-connected if it
contains no holes of boundary-dimension $d \le n$. In general, a space contains
a 1-dimensional-boundary hole if and only if it is not
[simply-connected](https://en.wikipedia.org/wiki/Simply-connected). Hence,
simply-connected is equivalent to 1-connected. Hence, path-connected is
equivalent to 0-connected. The existence of a 0-dimensional hole is equivalent
to the space being empty. A
[ball](https://en.wikipedia.org/wiki/Ball_%28mathematics%29) has no holes of
any dimension. Therefore, its connectivity is infinite.

## Projective space

Arose from effects of perspective in arts. Also to properly deal with infinite
points that disturbed some people. Lines intersect at one point except when
they are parallel. We can imagine that those also meet/intersect at infinity
so that we can say uniformly all lines intersect once. But for that, negative
and positive infinity have to be the same. They need to be one point. So a
construction that realizes this is projective space.

Also, we consider everything up to scalars here. All points on a line are some
scalar times another point on that line. So, we can say projective space is a
space whose elements are lines, or it's a space whose elements are points (one
representative point for each line). Each point represents an equivalence
class. For example, $\mathbb{RP}^n$ or $P_n(\mathbb{R})$ is the real projective
space of $\mathbb{R}^{n+1}$. For $n=1$, the projective space of the plane is
the circle.

## Fundamental group

FG is a homotopy invariant. An invariant characterizing manifolds to compare
them. If two manifolds have different FG, they are not homotopic. If same, they
can be or cannot be homotopic. A manifold with no holes has trivial FG. The
circle has FG isomorphic to $\mathbb{Z}$, the set of all integers. Generators
are winding around the circle. Each winding number is basically a group
element. A disc with $n$ holes has FG the free group with $n$ generators. The
curves winding around each hole are the generators here. They form a group
structure. FG is also called the first homotopy group. FG of $S^2$ is trivial
since no holes.

FG of a product of path-connected spaces is the product of their FGs. The torus
is circle $\times$ circle.

FG of topological groups are commutative. FGs are not good at detecting
higher-dimensional structures.

A torus with 2 genus has an octagon as polygon, 3 genus will be a 12-gon.

## Homotopy

Homeomorphism is a cts. map which is a bijection and its inverse is also cts.
Homotopy is weaker than homeomorphism. There are different notions of
equivalence in topology. Homotopy equivalence is counting holes in different
spaces. Or homotopy equivalent if and only if deformation retracts (or
homeomorphic to def. retracts) of the same space. Deformation retraction is a
cts. process where you can squish but not beyond the holes.

Maps or spaces can be homotopic. So there can be a mapping between two spaces,
or we can think of the mapping itself as being cts. so that initially the
mapping is to the first space and finally to the second space. It's a cts.
family of maps. Homology and cohomology are invariant under homotopy. Circle
and Möbius strip are homotopic but not homeomorphic. Homotopy equivalent spaces
means FGs are isomorphic.

## Chain complexes

An [algebraic structure](https://en.wikipedia.org/wiki/Algebraic_structure)
that consists of a sequence of [abelian
groups](https://en.wikipedia.org/wiki/Abelian_group) (or
[modules](https://en.wikipedia.org/wiki/Module_%28mathematics%29)) and a
sequence of
[homomorphisms](https://en.wikipedia.org/wiki/Group_homomorphism) (also called
boundary operators or differentials) between consecutive groups such that the
[image](https://en.wikipedia.org/wiki/Image_%28mathematics%29) of each
homomorphism is included in the
[kernel](https://en.wikipedia.org/wiki/Kernel_%28algebra%29#Group_homomorphisms)
of the next.

Associated to a chain complex is its
[homology](https://en.wikipedia.org/wiki/Homology_%28mathematics%29), which
describes how the images are included in the kernels. The composition of any
two consecutive maps is zero. Index $n$ is the dimension of the vector space
formed by the complexes $C_n$. Elements of $C_n$ are chains and the kernel is
called cycle. Image is boundary. A chain complex whose homology groups are all
zero is called an exact complex or exact sequence.

## Homology

A cycle is a closed submanifold. A boundary is a subset of a cycle which is
also the boundary of a submanifold. A homology class is an equivalence class of
cycles modulo boundaries, and a homology class represents a hole. A homology
class is thus represented by a cycle which is not the boundary of any
submanifold: the cycle represents a hole, namely a hypothetical manifold whose
boundary would be that cycle, but which is "not there".

When the underlying object has a geometric interpretation as topological spaces
do, the $n$th homology group represents behavior in dimension $n$. Cutting a
manifold along a cycle homologous to zero separates the manifold into two or
more components. For example, cutting the sphere along a produces two
hemispheres. All closed surfaces can be produced by gluing the sides of some
polygon. When two cycles can be continuously deformed into each other, then
cutting along one produces the same shape as cutting along the other, up to
some bending and stretching. In this case the two cycles are said to be
homologous or to lie in the same homology class.

Since each chain group $C_n$ is abelian all its subgroups are normal. Then
because $\ker(\partial_n)$ is a subgroup of $C_n$, $\ker(\partial_n)$ is
abelian, and since $\operatorname{im}(\partial_{n+1}) \subseteq
\ker(\partial_n)$ therefore $\operatorname{im}(\partial_{n+1})$ is a [normal
subgroup](https://en.wikipedia.org/wiki/Normal_subgroup) of
$\ker(\partial_n)$. Then one can create the [quotient
group](https://en.wikipedia.org/wiki/Quotient_group)

$$
H_n(X) := \ker(\partial_n)\,/\,\operatorname{im}(\partial_{n+1})
        = Z_n(X)\,/\,B_n(X),
$$

called the $n$th homology group of $X$. The elements of $H_n(X)$ are called
homology classes. Each homology class is an equivalence class over cycles, and
two cycles in the same homology class are said to be homologous.

Looks for objects without boundary which are not the boundary of an object. The
first part focuses on closed loops and not open paths; the second part says it
should not bound a patch. In a torus, 1D (co)homology has two generators.

Homology theory attaches vector spaces or groups to topological structures.

Homology groups are the abelianization of homotopy groups. Only the first
homology group is non-abelian (FG). All higher ones are abelian. All homology
groups are abelian. By adding commutativity to homotopy, we are losing
information but simplifying things in homology. Homology groups detect holes
and can tell winding numbers around holes, but homotopy groups do much more.
They in addition can tell how loops wind around the holes and how they compose
in winding together. FG for a plane with two holes is the free group with two
generators, while $H_1$ is the free abelian group with two generators.

Two topological spaces that are [homotopy
equivalent](https://en.wikipedia.org/wiki/Homotopy_equivalent) have
[isomorphic](https://en.wikipedia.org/wiki/Group_isomorphism) homology groups.

The first homotopy group $\pi_1(X)$ is the group of directed loops starting and
ending at a predetermined point (e.g. its center). It is equivalent to the
[free group](https://en.wikipedia.org/wiki/Free_group) of rank 2, which is not
commutative: looping around the leftmost cycle and then around the rightmost
cycle is different than looping around the rightmost cycle and then looping
around the leftmost cycle. In contrast, its first homology group $H_1(X)$ is
the group of cuts made in a surface. This group is commutative, since
(informally) cutting the leftmost cycle and then the rightmost cycle leads to
the same result as cutting the rightmost cycle and then the leftmost cycle.

## Betti number

The $n$th Betti number represents the
[rank](https://en.wikipedia.org/wiki/Rank_of_a_group) of the $n$th [homology
group](https://en.wikipedia.org/wiki/Homology_group), denoted $H_n$. Only the
ranks of infinite groups are considered, so for example if $H_n(X) \cong
\mathbb{Z}^k \oplus \mathbb{Z}/(2)$, where $\mathbb{Z}/(2)$ is the [finite
cyclic group](https://en.wikipedia.org/wiki/Finite_cyclic_group) of order 2,
then $b_n(X) = k$.

The $k$th Betti number refers to the number of $k$-dimensional holes on a
topological surface. A "$k$-dimensional hole" is a $k$-dimensional cycle that
is not a boundary of a $(k+1)$-dimensional object. One 0-D hole means only one
connected component. Another interpretation of $b_k$ is the maximum number of
$k$-dimensional curves that can be removed while the object remains connected.

For the projective plane, however, the 1st Betti number is 0. This is because
$H_1(P)$ is a finite group — it does not have any infinite component. The
finite component of the group is called the torsion coefficient of $P$.
Intuitively, it corresponds to the fact that there is a single non-contractible
"loop", but if we do the loop twice, it becomes contractible to zero. This
phenomenon is called torsion. The (rational) Betti numbers $b_k(X)$ do not take
into account any [torsion](https://en.wikipedia.org/wiki/Torsion_subgroup) in
the homology groups.

If $X$ is an $n$-dimensional manifold, there is a symmetry interchanging $k$ and
$n-k$, for any $k$:

$$
b_k(X) = b_{n-k}(X),
$$

under conditions (a closed and oriented manifold); see [Poincaré
duality](https://en.wikipedia.org/wiki/Poincar%C3%A9_duality).

The Euler characteristic is the alternating sum of Betti numbers.

## Cohomology

Instead of looking for subspaces detecting holes, cohomology assigns a real
value to each object in our space. Differential forms a local valuation in each
point and each direction. De Rham cohomology studies these differential forms
and a so-called exterior derivative $d$.

So for our cohomological search of holes, we must find closed forms which are
not exact. We are looking for forms whose exterior derivative is zero that are
not the exterior derivative of some other form. A differential form is closed
if its derivative is zero, and it's exact if it is the derivative of something
else. The derivative of a derivative is zero, which means the boundary of a
boundary is always zero. Being exact is like bounding a patch and being closed
is like having no boundary. A hole is a closed form which is not exact. The
$k$-dimensional De Rham cohomology of a space is the quotient of the space of
closed $k$-forms by the space of exact $k$-forms.

The $k$th homology group is isomorphic to the $(n-k)$th cohomology group, $n$
being the dimension of the manifold. Instead of starting from chain complexes
and extracting boundaries and reducing dimensions one by one, we add a
dimension in every step in cohomology. It's the other way around.

## Fibre bundles

## Tangent bundles

## Principal bundles

## Connection

It makes precise the idea of transporting local geometric objects, such as
tangent vectors or tensors in the tangent space, along a curve or family of
curves in a parallel and consistent manner. There are various kinds of
connections in modern geometry, depending on what sort of data one wants to
transport.

For instance, an [affine
connection](https://en.wikipedia.org/wiki/Affine_connection), the most
elementary type of connection, gives a means for parallel transport of [tangent
vectors](https://en.wikipedia.org/wiki/Tangent_space) on a
[manifold](https://en.wikipedia.org/wiki/Manifold) from one point to another
along a curve. An affine connection is typically given in the form of a
[covariant derivative](https://en.wikipedia.org/wiki/Covariant_derivative),
which gives a means for taking [directional
derivatives](https://en.wikipedia.org/wiki/Directional_derivative) of vector
fields. Thus a covariant derivative is a way of specifying a
[derivative](https://en.wikipedia.org/wiki/Derivative) of a vector field along
another vector field on a manifold.
