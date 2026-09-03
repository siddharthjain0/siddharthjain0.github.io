Physical lattice models as a testbed for real-world quantum networks. This page collects the work presented as a poster at **IEEE Quantum Week (QCE) 2026** — *Multipartite entanglement characterization in quantum networks from spin clusters*, with Zhehao Dai and Kaushik P. Seshadreesan.

<p class="pub-links"><a href="qce2026-poster.pdf">Poster (PDF)</a> <a href="FORM_URL" target="_blank" rel="noopener">Send feedback</a> <a href="mailto:sij50@pitt.edu?subject=QCE%202026%20poster">Email me</a></p>

## Why look at a spin model

Multiparty protocols — conference key agreement, distributed quantum computing, secret sharing — need entanglement shared among three or more parties at once, not just pairs. A natural question follows: what does a large network carrying that kind of entanglement actually look like? Which nodes become hubs, and how far do the multiparty links reach?

Nobody can build one at that scale yet to go and measure it. So the alternative is to compute one. A disordered quantum magnet at its critical point has a ground state made of many independent GHZ clusters, each a small piece of genuine multiparty entanglement. Turning those clusters into network links gives a structure we can study at large sizes.

Earlier work built exactly this model but kept only the *pairwise* links — clusters touching two nodes — and discarded everything else. The discarded part is the multipartite resource. This project characterizes it.

## How the network is built

The starting point is the random transverse-field Ising model on an $N = L \times L$ lattice,

$$\mathcal{H} = -\sum_{\langle ij\rangle} J_{ij}\,\sigma_i^{x}\sigma_j^{x} - \sum_{i} h_i\,\sigma_i^{z},$$

at its critical point. A strong-disorder renormalization group (SDRG) procedure running in $O(N\log N)$ time returns the ground state as a collection of independent GHZ states.

Circular nodes with radii drawn from a power law are then packed onto the lattice. A GHZ cluster overlapping two or more nodes becomes a **hyperedge**, whose size is the number of nodes it spans. Hyperedges of size $\ge 3$ are the multipartite resources; throwing them away recovers the pairwise network studied previously. The **hyperdegree** of a node is the number of distinct clusters it belongs to.

![Node-packing geometry, with colour encoding relative node radius.](figures/packing.png "medium")
*Node-packing geometry. Colour encodes relative node radius.*

## What we found

Only about **10% of hyperedges are multipartite**, yet those few reach roughly **40% of all nodes**. Both ratios stay roughly constant up to $L = 4096$. The multipartite layer is sparse but does a large share of the connecting.

The hyperdegree distribution is heavy-tailed, with an exponent inside the $2 < \gamma < 3$ window — the regime associated with scale-free behaviour, meaning the network has hubs rather than a typical degree. The hyperedge-size distribution is also heavy-tailed, but with a steeper exponent.

![Hyperdegree distribution on log-log axes, following a power law.](figures/total_hyperdegree.png "medium")
*Hyperdegree distribution.*

![Hyperedge-size distribution on log-log axes.](figures/hyperedge_size.png "medium")
*Hyperedge-size distribution.*

## Structure beyond the distributions

An obvious objection: if the interesting content is just two power laws, why not build an abstract hypergraph with the same distributions and skip the physics entirely?

We tested that directly, against a configuration-model null — same hyperdegree distribution, same hyperedge-size distribution, wiring otherwise randomized. The real network is significantly **more disassortative** than the null, and the discrepancy *grows* with system size: roughly $4\sigma$ per sample at $L = 1024$, in all 50 samples, while the largest-component size matches the null almost exactly (so it is not a connectivity artifact).

That null model *is* the abstract matched-distribution hypergraph. It does not reproduce this structure, which is the empirical answer to the objection: the physics is putting something there that the marginals alone do not imply.

## Scope and what is next

This is a physically-grounded generative model, not a hardware proposal, and the structure is not claimed to be that of any existing quantum network. The point is to give the multipartite regime a tractable testbed where complex topology *emerges* from a real Hamiltonian instead of being imposed by hand, and to check what that buys against the null models the network-science community already uses.

Currently in progress: robustness and long-range connectivity of the multipartite layer — if the hubs are removed, does the multiparty network fragment, and can it carry entanglement over long distances? That is what decides whether this structure is useful for protocols rather than merely present. A rigorous entanglement-criterion check for the larger clusters is also on the list.

## Feedback

If this connects to your own work, if you think something here is wrong, or if you would like to know when the preprint appears, I would like to hear from you.

<p class="pub-links"><a href="FORM_URL" target="_blank" rel="noopener">Share feedback or an idea</a> <a href="mailto:sij50@pitt.edu?subject=QCE%202026%20poster">sij50@pitt.edu</a></p>
