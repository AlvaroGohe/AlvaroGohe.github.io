---
layout: post
title: What is my research about?
date: 2026-07-28 16:11:00-0400
tags: pictures
images:
  compare: true
  slider: true
---

  <!-- ── Intro ── -->
  <p>
    My area of research is a field of pure mathematics known as <strong>algebraic geometry</strong>.
    Specifically, I study a class of structures called <strong>algebraic surfaces</strong>, which are
    two-dimensional geometric objects defined by polynomial equations.
  </p>

  <figure class="narrow">
    <img src="/assets/img/research_statement_pictures/Shapes.png" alt="The cylinder, the sphere and the cone" />
    <figcaption>
      The cylinder, the sphere and the cone are all algebraic surfaces as they can all be represented
      as sets of points in space whose coordinates $$(x,y,z)$$ satisfy a polynomial equation.
    </figcaption>
  </figure>

  <p>
    As a geometer, I am interested in analysing which properties these surfaces share and which
    properties allow us to tell them apart. For instance, there is a clear difference between the
    sphere and the cone. While the surface of the sphere is smooth and uniform, the cone has a
    pointy tip, which is what we call a <strong>singular point</strong>. Surfaces without singular
    points, like the sphere, are called <strong>smooth surfaces</strong>, whereas those with singular
    points, like the cone, are called <strong>singular surfaces</strong>.
  </p>

  <!-- ── K3 & Kummer ── -->
  <p>
    I specialise in studying the singular points of a particular class of surfaces known as
    <strong>K3 surfaces</strong>. These surfaces are of interest not only to mathematicians but also
    to physicists, as they play a key role in certain formulations of string
    theory.<sup class="cite"><a href="#ref1">[1]</a></sup> In particular, my research focuses on a
    class of K3 surfaces with multiple singular points, known as
    <strong>generalised Kummer surfaces</strong>.
  </p>

  <p>
    In general, finding surfaces with many singular points is a challenging problem. One fruitful
    approach involves examining the possible symmetries of simpler surfaces. For example, consider
    the symmetry of the plane that rotates all points by an angle of 180° around a point.
  </p>

  <figure class="full">
    <img src="/assets/img/research_statement_pictures/Carp_diagram.png" alt="180° rotation of the plane" />
  </figure>

  <p>
    If we identify the points in the plane that are related by this rotation, the resulting surface
    is a cone, where the rotation's fixed point corresponds to the singular point.
  </p>

  <figure class="full">
    <img src="/assets/img/research_statement_pictures/Cone_carp.png" alt="Cone as a quotient of the plane" />
    <figcaption>
      This can be demonstrated by cutting a slit in a piece of paper and folding it to bring each
      pair of symmetric points together.
    </figcaption>
  </figure>

  <p>
    In this case, we say that the cone is the <strong>quotient</strong> of the plane by a 180°
    rotation. Similarly, the generalised Kummer surfaces I study are quotients of a class of
    surfaces called <strong>abelian surfaces</strong>.
  </p>

  <!-- Three Kummer surface images -->
  <div class="fig-row">
    <figure>
      <img src="/assets/img/research_statement_pictures/Kmm3c.png" alt="Generalised Kummer surface with 9 singular points" />
    </figure>
    <figure>
      <img src="/assets/img/research_statement_pictures/Kmm4c.png" alt="Generalised Kummer surface with 10 singular points" />
    </figure>
    <figure>
      <img src="/assets/img/research_statement_pictures/Kmm2c.png" alt="Generalised Kummer surface with 16 singular points" />
    </figure>
  </div>
  <p class="fig-row-caption">
    Examples of generalised Kummer surfaces with 9, 10 and 16 singular points.
  </p>

  <!-- ── Positive characteristic ── -->
  <p>
    How many singular points can a generalised Kummer surface have, and how intricate can they be?
    Since Kummer surfaces were first described in 1833, this question has attracted the attention of
    many mathematicians. In 1987, Toshiyuki Katsura provided a classification of the number and
    types of singular points of generalised Kummer surfaces.<sup class="cite"><a href="#ref2">[2]</a></sup>
    However, Katsura's classification was incomplete: while it held for surfaces defined by
    polynomials with complex coefficients, it did not extend to a setting called
    <strong>positive characteristic</strong>.
  </p>

  <p>
    Positive characteristic geometry studies geometric objects defined over number systems in which
    arithmetic is performed modulo a fixed prime number $$p$$, for example, $$p = 2, 3, 5$$ or $$7$$.
    This is similar to clock arithmetic, where numbers "wrap around" after reaching $$12$$. In these
    number systems, the arithmetic is quite surprising — for instance, $$1 + 1 = 0$$ and
    $$(a+b)^2 = a^2 + b^2$$ when $$p = 2$$. This changes many geometric properties, often making
    features of surfaces like singularities and symmetries behave in fundamentally different ways
    from the classical setting, which is known as <strong>characteristic zero</strong>.
  </p>

  <p>
    The most important result of my thesis is the complete classification of all possible singular
    points of generalised Kummer surfaces in positive characteristic. I originally proved this
    result under certain technical assumptions, but since I defended my thesis, I have managed to
    remove these conditions. I am currently preparing this result for publication, and it has
    already attracted interest from researchers in the field, who have inquired about the details
    of the proof.
  </p>

  <!-- ── Good reduction ── -->
  <p>
    One reason researchers are interested in positive characteristic geometry is that many problems
    are simpler in this setting. This is because, unlike in characteristic zero — where surfaces
    typically contain infinitely many points — surfaces in positive characteristic usually have only
    a finite number of points. These points encode important information about the geometry of the
    surface and can be studied efficiently using numerical methods.
  </p>

  <p>
    Given a smooth surface $$S$$ in characteristic zero, there is a process called
    <strong>reduction modulo $$\mathfrak{p}$$</strong> that produces a surface $$S_\mathfrak{p}$$ in
    positive characteristic. If $$S_\mathfrak{p}$$ is also smooth, we say that the surface has
    <strong>good reduction at $$\mathfrak{p}$$</strong>. Here, the letter $$\mathfrak{p}$$ stands for
    prime, because the possible ways of constructing these reductions are naturally associated with
    prime numbers. If $$S$$ has good reduction, then $$S$$ and $$S_\mathfrak{p}$$ share similar geometric
    features, so this provides an additional perspective for understanding surfaces in characteristic
    zero.
  </p>

  <figure class="full">
    <img src="/assets/img/research_statement_pictures/Good_reduction.png"
         alt="Good and bad reduction at various primes" />
    <figcaption>
      In this example, the surface has good reduction at $$\mathfrak{p} = 2, 3$$ and $$7$$, and bad
      reduction at $$\mathfrak{p} = 5$$.
    </figcaption>
  </figure>

  <p>
    If a surface has good reduction at all primes, it is said to have
    <strong>everywhere good reduction</strong>. These surfaces are extremely rare, and the few
    examples that we know are quite elaborate. In the paper
    <em>Explicit desingularisation of Kummer surfaces in characteristic two via specialisation</em>,
    I described the first known examples of K3 surfaces with everywhere good
    reduction.<sup class="cite"><a href="#ref3">[3]</a></sup> To give a sense of why such examples
    had not been discovered before, note that in 1990, Abrashkin proved that there are no K3
    surfaces with everywhere good reduction whose equations have rational
    coefficients.<sup class="cite"><a href="#ref4">[4]</a></sup> To obtain these examples, I had to
    develop new techniques to analyse the reduction of K3 surfaces and employ computational methods
    to implement them.
  </p>

  <!-- ── Moduli spaces ── -->
  <p>
    During my PhD, I have also made contributions to the understanding of a class of geometric
    structures known as <strong>moduli spaces</strong>. Informally, these can be understood as
    follows. Suppose one wishes to study a collection of geometric objects — for example, triangles.
    If the collection satisfies certain conditions, one can associate a moduli space to it, which is
    a geometric structure whose points correspond to objects in the collection, arranged so that
    similar objects are represented by nearby points.
  </p>

  <figure class="full">
    <img src="/assets/img/research_statement_pictures/Triangles.png" alt="Moduli space of triangles" />
    <figcaption>
      The moduli space parametrising all triangles whose perimeter is one is, maybe surprisingly,
      also a triangle. Any family of triangles where the lengths of the sides vary continuously
      gives rise to a continuous path in the moduli space.
    </figcaption>
  </figure>

  <p>
    I am interested in the moduli space that parametrises objects called
    <strong>genus two curves</strong>. These curves are connected to my research because they can be
    used to construct abelian surfaces, in such a way that the symmetries of the curve induce
    symmetries of the surface. In the paper
    <em>Intersections of the automorphism and Ekedahl–Oort strata inside the moduli space of genus
    two curves</em>, I gave a description of this moduli space in positive
    characteristic.<sup class="cite"><a href="#ref5">[5]</a></sup> The main result is that this
    moduli space is three-dimensional and admits a decomposition into lower-dimensional pieces,
    called <strong>strata</strong>, which correspond to families of curves with special properties.
  </p>

  <!-- ── Cryptography ── -->
  <p>
    As a researcher working in pure mathematics, it is often difficult to anticipate what possible
    applications your area of research may have. In my case, however, there is a clear connection
    between positive characteristic geometry and cryptography. The abelian surfaces I discussed
    earlier are a generalisation of another geometric object called <strong>elliptic curves</strong>,
    which are widely used in cryptographic applications.
  </p>

  <p>
    Elliptic curve cryptography is a standard method for securing Internet connections and
    end-to-end encrypted messaging, but it is unfortunately vulnerable to potential quantum attacks.
    This has prompted interest in developing new algorithms that will remain secure in the era of
    quantum computers. One of these protocols involving elliptic curves, called Supersingular
    Isogeny Diffie–Hellman (SIDH), was considered secure until 2022, when Castryck and Decru
    described an attack that exploits abelian and Kummer surfaces in positive characteristic to
    recover encoded information.<sup class="cite"><a href="#ref6">[6]</a></sup>
  </p>

 <!-- ── References ── -->
  <div class="references">
    <h2>References</h2>
    <ol>
      <li id="ref1">
        P. S. Aspinwall, "K3 surfaces and string duality," in
        <em>Theoretical Advanced Study Institute in Elementary Particle Physics (TASI 96):
        Fields, Strings, and Duality</em>, pp. 421–540, 1996.
        arXiv:<a href="https://arxiv.org/abs/hep-th/9611137" target="_blank">hep-th/9611137</a>.
      </li>
      <li id="ref2">
        T. Katsura, "Generalized Kummer surfaces and their unirationality in characteristic $$p$$,"
        <em>Journal of the Faculty of Science of the University of Tokyo, Sect. IA, Math.</em>,
        vol. 34, pp. 1–41, 1987.
      </li>
      <li id="ref3">
        A. Gonzalez-Hernandez, "Explicit desingularisation of Kummer surfaces in characteristic
        two via specialisation," <em>Journal of Symbolic Computation</em>, vol. 135, p. 102541,
        2026. DOI: <a href="https://doi.org/10.1016/j.jsc.2025.102541" target="_blank">10.1016/j.jsc.2025.102541</a>.
      </li>
      <li id="ref4">
        V. A. Abrashkin, "Modular representations of the Galois group of a local field, and a
        generalization of the Shafarevich conjecture,"
        <em>Mathematics of the USSR-Izvestiya</em>, vol. 35, no. 3, pp. 469–518, 1990.
      </li>
      <li id="ref5">
        A. Gonzalez-Hernandez, "Intersections of the automorphism and the Ekedahl–Oort strata
        in $$M_2$$," <em>arXiv</em>, 2025.
        <a href="https://arxiv.org/abs/2507.07278" target="_blank">arXiv:2507.07278</a>.
      </li>
      <li id="ref6">
        W. Castryck and T. Decru, "An efficient key recovery attack on SIDH,"
        <em>Cryptology ePrint Archive</em>, 2022.
        <a href="https://eprint.iacr.org/2022/975" target="_blank">eprint.iacr.org/2022/975</a>.
      </li>
    </ol>
  </div>

