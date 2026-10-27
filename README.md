I work in program management at a deep-tech hardware company. Outside work I run language models
on my own machine and send fixes to open-source AI software.

## Open source

Pull requests and bug reports to projects I use. States as of 28 October 2026; the date is the
merge or closing date, or the opening date of what is still open.

### [oMLX](https://github.com/jundot/omlx)

An LLM inference server for Apple silicon. 3 pull requests merged, 1 open, 4 issues.

#### Pull requests

| Ref | What | State | Date |
| --- | --- | --- | --- |
| [#2161](https://github.com/jundot/omlx/pull/2161) | Calibrate models larger than RAM: the quantiser streams the model one layer at a time. About 3,000 lines. | Merged | 2026‑09‑16 |
| [#2159](https://github.com/jundot/omlx/pull/2159) | Fix the decoding of MXFP8 block scales in dequantisation. | Merged | 2026‑07‑10 |
| [#2140](https://github.com/jundot/omlx/pull/2140) | Ship the calibration data inside the package. | Merged | 2026‑07‑09 |
| [#3504](https://github.com/jundot/omlx/pull/3504) | Grammar-constrained output that keeps speculative decoding on. | Open | 2026‑09‑07 |

#### Issues

| Ref | What | State | Date |
| --- | --- | --- | --- |
| [#2238](https://github.com/jundot/omlx/issues/2238) | Mixture-of-experts decoding ran at 34% of the memory roofline, against 94% for a dense model, on an M3 Ultra. | Closed | 2026‑09‑24 |
| [#3507](https://github.com/jundot/omlx/issues/3507) | The embeddings endpoint answered 200 with vectors full of nulls when the model returned NaN. | Closed | 2026‑09‑12 |
| [#3505](https://github.com/jundot/omlx/issues/3505) | The memory guard sets custom tiers to a soft limit of 0.85 and gives no setting for prefill headroom. | Open | 2026‑09‑07 |
| [#3506](https://github.com/jundot/omlx/issues/3506) | The native 8-bit affine kernel for Qwen3.5 cannot engage during prefill, because of its threshold against the chunk size. | Open | 2026‑09‑07 |

### [Omi](https://github.com/BasedHardware/omi)

Open-source AI that sees your screen and listens to your conversations. 3 pull requests merged,
each stopping duplicate action items.

| Ref | What | State | Date |
| --- | --- | --- | --- |
| [#7092](https://github.com/BasedHardware/omi/pull/7092) | Deduplicate when a staged task is promoted. | Merged | 2026‑06‑10 |
| [#7093](https://github.com/BasedHardware/omi/pull/7093) | Make creating an action item idempotent with a content hash. | Merged | 2026‑06‑09 |
| [#7091](https://github.com/BasedHardware/omi/pull/7091) | Sync: adopt orphan action items by description. | Merged | 2026‑06‑05 |

### Also

- [mlx-embeddings #80](https://github.com/Blaizzy/mlx-embeddings/issues/80), open: a bug report.
  Padded ModernBERT batches return NaN embeddings when the longest sequence is a multiple of 32
  tokens, at 128 tokens or more.
- [Nimbalyst #1161](https://github.com/nimbalyst/nimbalyst/pull/1161), open: adds Kimi Code as an
  agent provider.

## How I work

Most of the code I write now, I write with AI coding agents; I direct them, review what they
produce and test it before it goes out under my name.

More about me, and how to reach me: [cnob.me](https://cnob.me).
