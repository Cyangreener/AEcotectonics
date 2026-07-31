# AEcotectonics

*How AEco organizes itself, the architectonic discipline of tiers, modules, primitives, and dependencies.*

This repository does not contain AEco's claims about economics or governance. It contains the **rules those claims must follow**. It is the structural constitution of the Automated Economy Initiative: the specification of how the framework is built, how its parts are admitted, and how they are kept from silently contradicting one another. The content lives in `AEco_Skeleton`. This is the discipline that governs it.


## The problem this repository exists to solve

AEco studies a phenomenon with thousands of intersecting facets. Labor, value, capital, authority, allocation, legitimacy, information, agency, each is its own subject, with its own assumptions, its own parameters, its own literature. Any framework that means to say something true about the whole must eventually say something about a great many of these at once, and about the places where they intersect, because it is precisely at the intersections that the interesting conditions arise: authority *over* resources, value *under* automation, legitimacy *of* allocation.

This creates a problem that is easy to underestimate and fatal if ignored. When a large body of work grows one piece at a time, each piece locally reasonable, each addition justified on its own terms, the pieces can come to rest on **mutually incompatible assumptions** without anyone noticing. No single author holds the entire structure in view at once, so a claim made carefully in one place can quietly presuppose something that a claim made carefully in another place denies. The individual parts are sound. Their combination is not. And because the contradiction lives *between* the parts rather than inside any one of them, ordinary care within each part cannot catch it.

This is not a failure of rigor. It is the structural condition of interdisciplinary work. A framework that reaches across many domains inherits the coherence problem of *all of them at once*, and the wider it reaches, the more places two of its commitments can silently disagree. The temptation, felt by every ambitious framework, is to keep reaching: to add one more domain, one more distinction, one more starting assumption, because each is useful and each seems harmless. The cost is never paid at the moment of the addition. It is paid later, all at once, when the accumulated structure turns out not to hold together, and by then it is expensive to repair, because so much has been built on top of the parts that were quietly in conflict.

A framework can die this way without ever being wrong about any single thing. It dies of incoherence, not error.


## Two ways a system can grow

There are two fundamentally different ways to assemble a large intellectual structure, and the distinction is the whole point of this repository.

A structure can grow by **aggregation**, parts added because they are useful, held together by the fact that each seemed like a good idea at the time. The relations between the parts are whatever they happen to be. New parts are admitted whenever a need is felt. This produces something that can look complete and even elegant, but its coherence is accidental: it holds together only as far as the author's memory and good sense reach, and no further. There is no principle that determines whether a given part *belongs*, so there is no principle that can be violated, which means there is nothing to catch the contradiction when it comes.

A structure can instead grow **architectonically**, where every part derives its place from an idea of the whole, and no part is admitted except as the whole requires it. Here the relations between parts are not incidental; they are the very thing that determines what the parts *are*. A component exists because the structure necessitates it, occupies the position the structure assigns it, and connects to exactly the other components the structure demands. Admission is governed. Necessity, not usefulness, is the criterion. And because there is now a principle governing what belongs, there is something definite to check, and something definite that can fail, visibly, when a proposed part does not in fact follow.

The first kind of structure cannot be validated, because it has no rule to validate against. The second kind can. **AEco is committed to the second kind, without exception.** This repository states the commitment and the machinery that enforces it.


## What the repository specifies

The architectonic discipline of AEco rests on a small number of interlocking rules. Each is stated fully in its own document; what follows is the shape of the whole.

**Admission by necessity.** No primitive, no term, no component enters AEco because it is convenient, familiar, or borrowed from an adjacent field. A primitive is admitted only when it can be shown to be genuinely irreducible, underivable from what is already present. Everything that *can* be constructed from existing terms *must* be constructed, never assumed. The number of primitives is therefore not chosen; it is discovered, by finding the exact points at which construction from the existing base becomes impossible. Each such point is a candidate primitive, and each candidate must earn its place by a demonstration that it cannot be reduced. This is the single most important rule, because it is the one that keeps the framework a system that *derives* its content rather than a catalogue that *assumes* it.

**Tiers as genuine boundaries.** The framework is layered, and the layers are not merely folders. Each tier is meant to be intelligible through the tier immediately beneath it, without reaching all the way down to the foundation. A higher component depends on the *conclusions* of lower ones through a stable interface, not on their internal workings. When this holds, complexity is absorbed layer by layer and the structure stays tractable no matter how large it grows. When it fails, when a high component must reach back down to first principles to be understood, the layering is decorative and the complexity is not actually being managed. The tier discipline is the test that keeps the abstraction real.

**Modules with a shared spine.** Components are specified along a common set of axes, so that any two components are described in the same terms and are therefore comparable, composable, and checkable against one another. Sub-components inherit this spine and specialize it; they do not invent private structures that cannot be related back to the whole. The axes themselves are not imported from convenience or from a neighboring discipline, they are derived from AEco's own primitives, so that the framework's way of describing its parts is itself a consequence of the framework rather than an assumption layered on top of it.

**Declared and validated dependencies.** Every component states what it depends on. These declarations are not documentation; they are checked. A component that claims to build on another must genuinely follow from it, and a structure that declares a dependency it does not honor, or that quietly depends on something it never declared, is caught. This is what converts the architectonic commitment from an aspiration into an enforced property. The rule that parts must derive their place from the whole is worth stating only if violations of it can be detected; the dependency machinery is how they are detected.

Together these rules mean that AEco cannot grow by aggregation even if its author is tired, distracted, or tempted. A part that does not follow cannot be admitted; a contradiction between parts is surfaced rather than buried; the reach of the framework is bounded not by taste but by what the structure can actually support. The discipline does for the framework what no author's vigilance can do reliably on its own: it holds the whole in view at once, mechanically, on every change.

## The synthesis this repository draws on

The discipline described here is not invented from nothing. It is a synthesis of four traditions, each contributing a distinct and non-overlapping thing, and the synthesis matters more than any single source.

**Ontology**, the study of what kinds of things exist in a domain and what makes them the things they are, supplies the account of AEco's *components*: what a State is, what an Agent is, what distinguishes one kind of component from another, and what identity and category conditions each must satisfy. It answers *what the parts are*.

**Architectonics**, in the Kantian sense, the doctrine that systematic knowledge grows from an idea of the whole rather than by accumulation, supplies the account of *why the parts hang together*: the principle of admission, the criterion of necessity, the distinction between a system and a mere pile. It answers *why a given part belongs where it does, and whether it belongs at all*.

**Systems design**, the engineering discipline of decomposition, interfaces, abstraction, and composition, supplies the account of *how the structure scales*: how layers hide complexity, how components couple through stable interfaces, how a large system stays comprehensible. It answers *how the whole remains tractable as it grows*.

**Formal logic and type theory**, the mathematics of specification and checkable derivation, supply the account of *how any of this is enforced*: how a component's requirements can be stated precisely enough that conformance is decidable, how a dependency can be checked rather than merely asserted, how consistency becomes a property a machine can verify rather than a hope the author maintains. It answers *how the discipline is made real instead of aspirational*.

These four are not alternatives; they are the four faces of a single method. Ontology says what the parts are. Architectonics says why they cohere. Systems design says how they scale. Type theory says how the coherence is checked. Remove any one and the method loses a capacity it cannot do without. Without ontology the parts are undefined; without architectonics their arrangement is arbitrary; without systems design the structure collapses under its own size; without formal checking the whole discipline reduces to a promise. AEco's architectonics is the operation of all four at once, on a single body of work.