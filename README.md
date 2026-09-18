# Knowing a Fact vs. Being Able to Act

**Separating declarative knowledge gaps from procedural competence gaps in a taught reasoning system.**

Stefan Ragland, Dominion Labs Research & Development. Published 13 January 2026.

- Paper (PDF): [`paper/knowledge-and-competence.pdf`](paper/knowledge-and-competence.pdf)
- Paper (web): <https://dmnlabs.org/research/knowledge-and-competence/>
- Contact: research@dmnlabs.org

## The argument

A taught system accumulates two kinds of mastery over a subject: the facts it holds, and the operations
it can carry out. Conflating them makes the system misread its own state, taking "I have not been told
this" for "I am not competent here" or the reverse, and the two call for opposite responses: acquisition
against practice. The paper measures them as independent axes and tests five hypotheses on a running
symbolic system, including whether a specific missing fact can be registered without disturbing the
competence estimate.

## The measurements

| What | Result | Data |
|---|---|---|
| The five hypotheses, re-run 18 September 2026 | 16 of 16 checks pass. Teaching three connected facts moved declarative coverage 0.2293 to 0.2925 with procedural competence unchanged at 0.500; a missing in-subject relation registered exactly one acknowledged unknown, with two negative controls firing no false gap | [`data/dom-kg-01.json`](data/dom-kg-01.json) |
| Behaviour under a third deficit: evidence that does not determine a hypothesis | across 32 inductions, asserting on any one surviving hypothesis gives 26 assertions of false cases out of 192; asserting only what every hypothesis supports gives 0, while still asserting 73% of true cases | [`data/undetermined-evidence.json`](data/undetermined-evidence.json) |
| What closes that deficit | the one case the system asks for closes it in 16 of 16 inductions, in a mean of 2.6 rounds; randomly chosen further examples close 1 of 16 | [`data/closing-undetermined-evidence.json`](data/closing-undetermined-evidence.json) |

Each file is the manifest its run wrote, unedited. The ambiguity studies are reported in full in a
companion paper ([repository](https://github.com/DominionLabsInc/perceive-induce-name),
[paper](https://dmnlabs.org/research/perceive-induce-name/)).

## Citation

```bibtex
@techreport{ragland2026knowing,
  title       = {Knowing a Fact vs. Being Able to Act: separating declarative knowledge gaps from procedural competence gaps},
  author      = {Ragland, Stefan},
  institution = {Dominion Labs},
  year        = {2026},
  month       = {1},
  url         = {https://dmnlabs.org/research/knowledge-and-competence/}
}
```

## License

The paper and the data are released under [Creative Commons Attribution 4.0](LICENSE). Please cite the
paper if you use them.
