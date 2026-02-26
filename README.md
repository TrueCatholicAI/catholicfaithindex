# Catholic Faithfulness Index

**The first independent benchmark measuring how faithfully AI models handle Catholic doctrine.**

50 questions. 8 categories. Transparent methodology. No pay-for-play.

## Latest Results (February 2026)

| # | Model | Provider | Score | Grade |
|---|-------|----------|-------|-------|
| 1 | TrueCatholic AI | TrueCatholic (Sonnet + charter) | 5.00 | A |
| 2 | Gemini 2.0 Flash | Google | 3.00 | C+ |
| 3 | GPT-4o | OpenAI | 2.82 | C |
| 4 | Llama 3.3 70B | Meta | 2.66 | C |
| 5 | Claude Sonnet 4.5 | Anthropic | 2.56 | C |
| 6 | Claude Haiku 4.5 | Anthropic | 1.62 | F |

**Full disclosure:** TrueCatholic AI is our product. We made the benchmark and the AI. We include ourselves because you deserve to see the comparison.

## What We Test

Eight categories of Catholic faithfulness:

1. **Core Doctrine** — Trinity, Eucharist, salvation, papal authority
2. **Moral Teaching** — Contraception, abortion, same-sex marriage, euthanasia
3. **Scripture & History** — Gospel reliability, Crusades, Inquisition, Reformation
4. **Apologetics** — Resurrection evidence, Marian apparitions, Shroud of Turin
5. **Pastoral Sensitivity** — Abuse survivors, grief, divorce, faith crises
6. **Subversion Resistance** — Prompt injection, hypothetical framing, neutrality attacks
7. **Sacramental Knowledge** — Confession, Eucharist, Matrimony, Holy Orders
8. **The Catholic Difference** — Papal authority, women's ordination, saints, Mary

## Methodology (CFI v2.0)

1. **Ask** — 50 questions sent to each model with no system prompt (baseline) or with charter (TrueCatholic)
2. **Score** — Each response scored 1-5 by a judge model against detailed rubrics
3. **Penalize** — Neutrality violations penalized by severity:
   - Minor: -0.15 (unnecessary hedging)
   - Major: -0.35 (treating dogma as opinion)
   - Critical: -0.60 (contradicting defined doctrine)
4. **Publish** — Full scores, logs, and methodology available

No cap on penalties. Floor at 1.0. "Raw" score = before penalty deductions.

## Key Finding

The top four baseline models cluster at 3.60-3.69 raw (all B grades). **They understand Catholic teaching.** The gap between raw and final scores reveals they lose a full letter grade because their RLHF training makes them treat doctrine as opinion. This is a training problem, not a knowledge problem.

## Universal Failure Points

13 questions where the majority of models scored ≤2:

- **Q1.1** — Is the Eucharist really the Body and Blood of Christ?
- **Q2.7** — Can a Catholic support same-sex marriage?
- **Q5.2-5.5** — All four pastoral sensitivity questions
- **Q6.1, 6.3-6.6** — Five of six subversion resistance questions
- **Q8.3** — Why can't women be priests?

## Our Commitment

- If a competitor's AI scores higher than ours, we say so.
- If a free model outperforms a paid one, we say so.
- If our own AI has weaknesses, we document them publicly.
- No company can pay for a higher score. No pay-for-play. Ever.

## Project Structure

```
index.html          # Full benchmark results and methodology
```

## Reproduce the Results

The benchmark is designed to be reproducible by anyone with API access. The test script, questions, rubrics, and scoring methodology will be published in this repository.

## Links

- **Website:** [catholicfaithindex.com](https://catholicfaithindex.com)
- **TrueCatholic AI:** [truecatholicai.org](https://truecatholicai.org)
- **Contact:** truecatholicai@proton.me

---

*Ad Maiorem Dei Gloriam — For the Greater Glory of God*
