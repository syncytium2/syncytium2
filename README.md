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

### On authorship

The ideas, decisions, and review in these repositories are mine; most of the code is
Claude's (Anthropic's Claude Code). I set the problems, made the calls — including
overriding rules the model had adopted — and merged nothing I hadn't reviewed. Agent
commits carry a `Co-Authored-By: Claude` trailer.

<!--
  DRAFT — things to check or fill in before this is settled:

  1. Affiliation. This says nothing about where you work. If you want the lab and the
     university named, add a line; if you'd rather the profile stay project-only, it's
     already correct as written.
  2. Publications. Nothing here links to any paper. A line pointing at ORCID, Google
     Scholar, or PubMed would be the obvious addition and would also help the sites get
     indexed.
  3. Contact. Deliberately omitted — tonydefazio.com carries a contact form, and the
     address deliberately appears nowhere on that page. Putting a literal address here
     would undo that, so if you want contact on the profile, link the form rather than
     the address.
  4. The "most of the code is Claude's" line is copied from the per-repo authorship notes
     in colonel_kernel and murderboard. Check you want it at profile level too, where it
     applies to everything rather than to one project.
-->
