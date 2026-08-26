## Tony DeFazio

Neuroendocrinology and calcium imaging. I build small, open-source instruments for
**measuring things in neuroscience data** — and for finding out when the measurement
doesn't hold.

The three instruments run in the browser — no install, no account, and nothing you load
is ever uploaded anywhere. The fourth is the review process that keeps the other three
honest.

**→ [tonydefazio.com](https://tonydefazio.com)**

---

### The instruments

| | | |
|---|---|---|
| **[Colonel Kernel](https://github.com/syncytium2/colonel_kernel)** | Recovers the shape that links action potentials to a calcium signal, from ground-truth spike times and a measured dF/F₀ trace — and says so when no single shape fits. | [kernel.tonydefazio.com](https://kernel.tonydefazio.com) |
| **[no_peak](https://github.com/syncytium2/no_peak)** | CLUSTER pulse detection for hormone time series (LH, GnRH, GH). A faithful port of Veldhuis & Johnson, validated point-by-point against both Igor Pro and the original Fortran. | [nopeak.tonydefazio.com](https://nopeak.tonydefazio.com) |
| **[bugarach](https://github.com/syncytium2/bugarach)** | Finds the moments when many cells fire together — and measures how often you're wrong, on a simulation built from your own recordings. Six coordination detectors lifted out of MATLAB. | [bugarach.tonydefazio.com](https://bugarach.tonydefazio.com) |
| **[murderboard](https://github.com/syncytium2/murderboard)** | An adversarial review harness for document deliverables: eleven reviewer roles that try to tear a draft apart before it ships. Vendored into the three above. | [murderboard.tonydefazio.com](https://murderboard.tonydefazio.com) |

### The through-line

A tool that flatters itself is worse than no tool.

An instrument will always return *an answer*, and the answer is easiest to trust exactly
when nobody has checked what it cost. So each of these reports its own failure modes as
loudly as its results — no_peak's front page leads with what CLUSTER **misses** (roughly
40% of true pulses), bugarach scores its detectors against planted events with known times
rather than against another detector's opinion, and Colonel Kernel is built to return "no
single kernel fits" rather than a plausible one.

The fourth exists to hold the other three to it.

### Publications

[ORCID 0000-0001-7302-7528](https://orcid.org/0000-0001-7302-7528) ·
[Bibliography](https://www.ncbi.nlm.nih.gov/myncbi/richard.defazio.1/bibliography/public/)

### On authorship

Provenance differs by project, so one line would be wrong for all four:

- **colonel_kernel** and **bugarach** began as my own MATLAB code. Claude (Anthropic's
  Claude Code) did the port, and does the coding now.
- **no_peak** is a port of Michael L. Johnson's CLUST5 Fortran. I wrote the Igor Pro port;
  Claude did Igor → web and Fortran → web.
- **murderboard** is Claude's code to my design.

Throughout: I set the problems, made the calls — including overriding rules the model had
adopted — and merged nothing I hadn't reviewed. Agent commits carry a `Co-Authored-By:
Claude` trailer.

<!--
  Settled 2026-08-25:
  - Affiliation: deliberately not named. Location dropped from the site masthead too.
  - Publications: ORCID + NCBI bibliography added above.
  - Contact: the form on tonydefazio.com. No literal address here or there, by design.
  - Authorship: rewritten per-project rather than one blanket line.

  DELIBERATELY NOT SAID HERE: that the no_peak port was made with Michael Johnson's
  approval. no_peak's own docs (docs/next-steps.md §1) record that this claim has no dated
  primary record, and its About page wording was narrowed on 2026-08-25 for that reason.
  Repeating it here would put an unverified claim about a named person on a second public
  surface. If a dated record ever exists, that is the moment to reconsider — not before.
-->
