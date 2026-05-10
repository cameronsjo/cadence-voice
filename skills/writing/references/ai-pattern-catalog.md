# Pattern Catalog: 32 Patterns to Detect and Fix

Based on Wikipedia's "Signs of AI writing" (WikiProject AI Cleanup), detection research from Science Advances, GPTZero, and Northeastern University stylometry studies.

Core insight: "LLMs use statistical algorithms to guess what should come next. The result tends toward the most statistically likely result that applies to the widest variety of cases."

---

## Content Patterns

### 1. Undue emphasis on significance, legacy, and broader trends

**Words to watch:** stands/serves as, is a testament/reminder, a vital/significant/crucial/pivotal/key role/moment, underscores/highlights its importance/significance, reflects broader, symbolizing its ongoing/enduring/lasting, contributing to the, setting the stage for, marking/shaping the, represents/marks a shift, key turning point, evolving landscape, focal point, indelible mark, deeply rooted

**Problem:** LLMs puff up importance by claiming arbitrary aspects represent or contribute to broader topics.

**Before:** The initiative was part of a broader movement across the industry to decentralize governance, marking a pivotal moment in the evolution of platform security.

**After:** The initiative decentralized security decisions to individual teams instead of routing everything through a central review board.

---

### 2. Undue emphasis on notability and media coverage

**Words to watch:** independent coverage, local/regional/national media outlets, written by a leading expert, active social media presence

**Problem:** LLMs hit readers over the head with claims of notability, listing sources without context.

**Before:** The framework has been featured in The New York Times, Wired, and The Verge, garnering significant attention.

**After:** In a 2024 Wired interview, the lead developer argued that the framework's approach to sandboxing was more practical than academic alternatives.

---

### 3. Superficial analyses with -ing endings

**Words to watch:** highlighting/underscoring/emphasizing..., ensuring..., reflecting/symbolizing..., contributing to..., cultivating/fostering..., encompassing..., showcasing...

**Problem:** AI tacks present participle phrases onto sentences to add fake depth.

**Before:** The new API reduces latency by 40%, showcasing the team's commitment to performance and highlighting the importance of efficient resource management.

**After:** The new API reduces latency by 40%. The main change was moving to connection pooling instead of per-request connections.

---

### 4. Promotional and advertisement-like language

**Words to watch:** boasts a, vibrant, rich (figurative), profound, enhancing its, showcasing, exemplifies, commitment to, natural beauty, nestled, in the heart of, groundbreaking (figurative), renowned, breathtaking, must-visit, stunning

**Problem:** LLMs can't maintain a neutral tone, especially for descriptive topics.

**Before:** The platform boasts a vibrant ecosystem of plugins, showcasing its commitment to extensibility and developer experience.

**After:** The platform has about 2,000 community plugins. The most-used ones handle auth, logging, and database migrations.

---

### 5. Vague attributions and weasel words

**Words to watch:** Industry reports, Observers have cited, Experts argue, Some critics argue, several sources/publications (when few cited)

**Problem:** AI attributes opinions to vague authorities without specific sources.

**Before:** Experts believe the tool plays a crucial role in the modern development ecosystem.

**After:** A 2024 Stack Overflow survey found 44% of professional developers use AI coding assistants at least weekly.

---

### 6. Outline-like "challenges and future prospects" sections

**Words to watch:** Despite its... faces several challenges..., Despite these challenges, Challenges and Legacy, Future Outlook

**Problem:** Formulaic "challenges" sections that add nothing specific.

**Before:** Despite its strengths, the framework faces challenges typical of open-source projects, including contributor burnout and funding. Despite these challenges, it continues to thrive.

**After:** The project lost two of its three core maintainers in 2024. A Linux Foundation grant in January 2025 funded one full-time developer.

---

## Language and Grammar Patterns

### 7. Overused AI vocabulary

**The kill list (high-frequency AI words):** Additionally, align with, crucial, delve, emphasizing, enduring, enhance, fostering, garner, highlight (verb), interplay, intricate/intricacies, key (adjective), landscape (abstract noun), pivotal, showcase, tapestry (abstract noun), testament, underscore (verb), valuable, vibrant

**Extended kill list:** leverage, harness, beacon, paradigm, multifaceted, nuanced, groundbreaking, seamless, holistic, robust, comprehensive, utilize, facilitate, realm, navigate (abstract), foster, nestled

**Frequency data (GPTZero, 3.3M texts):**
- "crucial role in" -> 182x more frequent in AI text than human
- "today's fast-paced world" -> 107x
- "aims to explore" -> 50x
- "delves" -> 28x spike in academic writing post-2023 (Science Advances)

**Fix:** Replace with plain English. "Crucial" -> "important" or just cut it. "Leverage" -> "use." "Landscape" -> name the actual thing. "Delve" -> never use this word.

---

### 8. Copula avoidance

**Words to watch:** serves as, stands as, marks, represents [a], boasts, features, offers [a]

**Problem:** LLMs substitute elaborate constructions for simple "is/are/has."

**Before:** The library serves as the primary interface for database connections. The config features four distinct modes and boasts full backward compatibility.

**After:** The library is the primary interface for database connections. The config has four modes and is backward-compatible.

---

### 9. Negative parallelisms

**Problem:** "Not only...but..." and "It's not just about..., it's..." are massively overused.

**Before:** It's not just about the syntax; it's about the developer experience. Not only does it reduce boilerplate, but it also improves readability.

**After:** The syntax is simpler and reduces boilerplate. Most developers I've talked to say that's the main reason they switched.

---

### 10. Rule of three overuse

**Problem:** LLMs force ideas into groups of three to appear comprehensive.

**Before:** The event features keynote sessions, panel discussions, and networking opportunities. Attendees can expect innovation, inspiration, and industry insights.

**After:** The event includes talks and panels. There's also time for informal networking between sessions.

---

### 11. Elegant variation (synonym cycling)

**Problem:** Repetition-penalty code causes excessive synonym substitution within a single passage.

**Before:** The tool processes incoming requests. The utility handles each payload. The system manages all throughput.

**After:** The tool processes incoming requests, handling each payload and managing throughput.

**The inverse — strategic term repetition:** In analytical writing, the fix for synonym cycling is not just "pick one synonym." It is to establish a key term with a precise definition and then reuse that exact term every time. If "scaffolding" means "the code wrapped around an AI model," write "scaffolding" 15 times. Do not alternate with "framework," "harness," or "wrapper" — each introduces ambiguity. Consistency signals precision in technical analysis; synonym cycling signals that the writer (or the model) is optimizing for lexical variety instead of clarity. See `references/craft-guide.md` "Strategic term repetition" for the full technique.

---

### 12. False ranges

**Problem:** "From X to Y" constructions where X and Y aren't on a meaningful scale.

**Before:** The impact spans from individual developer productivity to enterprise-wide transformation, from small scripts to massive codebases.

**After:** The tool works on projects of any size, though the benefits are most visible in large codebases where refactoring is tedious.

---

## Style Patterns

### 13. Em dash overuse

**Problem:** AI uses em dashes as a Swiss Army knife of punctuation. 3+ per paragraph is a strong tell.

**Before:** The term is promoted by vendors--not by practitioners. You don't see it in actual incident reports--yet this framing persists--even in official documentation.

**After:** The term is promoted by vendors, not by practitioners. You don't see it in actual incident reports, yet this framing persists in official documentation.

**Rule:** Max one em dash per paragraph. Replace the rest with commas, colons, semicolons, parentheses, or periods.

---

### 14. Overuse of boldface

**Problem:** AI emphasizes phrases in boldface mechanically, especially in lists.

**Before:** It combines **OKRs**, **KPIs**, and tools like the **Business Model Canvas** and **Balanced Scorecard**.

**After:** It combines OKRs, KPIs, and tools like the Business Model Canvas and Balanced Scorecard.

---

### 15. Inline-header vertical lists

**Problem:** Lists where items start with bolded headers followed by colons.

**Before:**
- **User Experience:** The interface has been redesigned for clarity.
- **Performance:** Load times improved through caching.
- **Security:** End-to-end encryption added.

**After:** The update redesigns the interface, improves load times through caching, and adds end-to-end encryption.

---

### 16. Title case in headings

**Problem:** AI capitalizes all main words in headings.

**Before:** ## Strategic Negotiations And Global Partnerships

**After:** ## Strategic negotiations and global partnerships

**Note:** Title case is acceptable in some style guides. Match the target publication's convention.

---

### 17. Emojis in professional content

**Before:**
🚀 **Launch Phase:** The product launches in Q3
💡 **Key Insight:** Users prefer simplicity

**After:** The product launches in Q3. User research showed a preference for simplicity.

---

### 18. Curly quotation marks

**Problem:** ChatGPT uses curly quotes instead of straight quotes. Minor but detectable.

**Fix:** Find-and-replace curly quotes with straight quotes if the target format uses straight.

---

## Communication Artifacts

### 19. Collaborative communication artifacts

**Words to watch:** I hope this helps, Of course!, Certainly!, You're absolutely right!, Would you like..., let me know, here is a...

**Problem:** Chatbot correspondence language gets pasted into content.

**Fix:** Delete entirely. These are never appropriate in published writing.

---

### 20. Knowledge-cutoff disclaimers

**Words to watch:** as of [date], Up to my last training update, While specific details are limited/scarce..., based on available information...

**Fix:** Delete and replace with actual sourced information or remove the claim.

---

### 21. Sycophantic/servile tone

**Before:** Great question! You're absolutely right that this is a complex topic. That's an excellent point.

**After:** The economic factors you mentioned are relevant here.

---

## Filler and Hedging

### 22. Filler phrases

| Filler | Replacement |
|---|---|
| In order to achieve this goal | To achieve this |
| Due to the fact that | Because |
| At this point in time | Now |
| In the event that you need | If you need |
| Has the ability to process | Can process |
| It is important to note that | (delete -- just state the thing) |
| In terms of | (recast the sentence) |
| At its core | (delete) |
| It's worth noting that | (delete) |

---

### 23. Excessive hedging

**Before:** It could potentially possibly be argued that the policy might have some effect on outcomes.

**After:** The policy may affect outcomes.

**Calibration rule:** Humans naturally vary certainty based on evidence. Be emphatic about things you know firsthand. Be tentative about things you've only read about. AI maintains uniform cautiousness regardless -- that uniformity is the tell.

---

### 24. Generic positive conclusions

**Before:** The future looks bright for the project. Exciting times lie ahead as the team continues their journey toward excellence. This represents a major step in the right direction.

**After:** The team plans to ship v2.0 by September with support for three new cloud providers.

---

## Professional Communication Patterns

These aren't AI vocabulary tells — they're interpersonal tells. Things a thoughtful human would catch on re-read but that AI produces by default when drafting professional communications. The brain treats social threats with the same intensity as physical ones (David Rock, SCARF model, 2008). Careless framing in a decline email or incident report triggers a real defensive response.

### 25. Implied follow-up that never happened

**Problem:** The framing implies you took actions you didn't. "Questions we couldn't resolve" implies you tried to resolve them — with the vendor present. If you didn't, the framing is dishonest.

**Before:** After careful review, there were questions we couldn't resolve about the integration path.

**After:** As we reviewed internally, we realized the integration path wasn't clear enough for our requirements.

**Fix:** State what you actually did. "We reviewed internally" is honest. "Questions we couldn't resolve" implies a conversation that never happened.

---

### 26. Invalidating framing

**Problem:** A sentence that makes the reader's effort sound pointless. Threatens the reader's Status and Fairness (SCARF). In a decline email, "we're solving this internally" tells the vendor their demo was a waste of everyone's time.

**Before:** We've decided to solve this internally with our existing tooling.

**After:** Any solution needs to integrate with our existing deployment pipeline — that path wasn't clear enough from the evaluation.

**Fix:** Frame the decision as YOUR requirements, not the reader's inadequacy. The reason should explain what you need, not what they lack.

---

### 27. Inference presented as observation

**Problem:** Stating a guess as if it were a fact. "Built for this engagement" was inference — the writer didn't know the vendor's development history. The Camera Test: could a camera record this? If not, it's interpretation.

**Before:** The demo appeared to be built specifically for this engagement.

**After:** We noticed a gap between the demo workflow and the architecture described in your documentation.

**Fix:** Describe what you observed (gap between demo and docs), not what you inferred (they built it just for you). See SKILL.md principle #9.

---

### 28. Filler affirmation after genuine content

**Problem:** A compliment followed by a generic affirmation that dilutes it. "The architecture impressed us. That's a real strength." The second sentence adds nothing — it just hedges the compliment with a safe label.

**Before:** Your monitoring approach was thorough. That's clearly an area of strength for the team.

**After:** Your monitoring approach was thorough — especially the automated anomaly detection that caught the simulated outage in under 90 seconds.

**Fix:** Trust the compliment. Either make it more specific or end it. Don't follow a genuine observation with a generic affirmation.

---

### 29. Generic warm closer

**Problem:** "We wish you the best" is the professional-email equivalent of "I hope this helps!" — a filler closer that signals the writer couldn't think of anything genuine. In the AI pattern catalog as pattern 19, but especially damaging in decline emails where it reads as dismissive.

**Before:** We wish you all the best in your future endeavors.

**After:** I'm going to try that anomaly detection approach in my homelab — it was genuinely impressive.

**Fix:** End with a personal action that proves engagement. Reference something specific from the interaction. If you can't think of anything specific, a clean "Thank you for your time" is better than a warm nothing.

---

### 30. Praise sandwich (manufactured cushioning)

**Problem:** AI routinely brackets criticism between manufactured praise: compliment, then the real message, then another compliment. Feedback research (Radical Candor) identifies this as "Ruinous Empathy" — the praise reads as insincere because it exists only to soften the blow. The reader learns to distrust all compliments because they might be cushions.

**Before:** Your presentation was really well-structured. One area for improvement: the data on slide 7 contradicted the conclusion on slide 12. Overall though, great energy and delivery!

**After:** The data on slide 7 contradicted the conclusion on slide 12 — the revenue numbers say growth but the churn chart says contraction. Which one is the real story? (Separately: the narrative arc of the deck was strong. That's worth preserving in the next version.)

**Fix:** Separate genuine praise from genuine criticism. Don't interleave them in a sandwich. Each should stand on its own. If you can only say one, say the criticism — that's what the reader needs.

---

### 31. Unsolicited advice disguised as observation

**Problem:** AI frequently generates "It might be worth considering..." or "One thing to keep in mind is..." — directive advice masquerading as neutral information-sharing. Distinct from hedging (pattern 23) because the issue isn't uncertainty; it's hiding a recommendation inside a descriptive frame to avoid the social cost of being direct.

**Before:** It might be worth considering whether the current approach scales beyond the initial use case. One thing to keep in mind is that similar systems have encountered performance bottlenecks at this scale.

**After:** This approach won't scale past 10k concurrent users. Here's why: [evidence]. I'd recommend [alternative].

**Fix:** If you have a recommendation, state it as a recommendation. "I recommend..." or "You should consider..." is honest. "It might be worth..." pretends you're just making an observation.

---

### 32. Enumerated comprehensiveness (forced exhaustive coverage)

**Problem:** AI tries to cover every possible angle rather than making editorial choices. Manifests as: exhaustive numbered lists ("here are 10 considerations"), equal-weight pros-and-cons regardless of actual balance, and "comprehensive frameworks" that name every factor without ranking any. Distinct from rule-of-three (pattern 10) — the symptom is not forced triads but forced completeness.

**Before:** There are several key considerations: (1) performance implications, (2) maintainability concerns, (3) team familiarity, (4) testing complexity, (5) documentation requirements, (6) migration path, (7) backwards compatibility, (8) monitoring needs, (9) cost implications, and (10) timeline impact.

**After:** Two things matter here: performance and migration path. The rest are manageable. Performance matters because [specific reason]. Migration is the risk because [specific reason].

**Fix:** Make choices. Rank. Say "the two things that matter are..." instead of listing ten. If everything is important, nothing is. Real experts prioritize; AI enumerates.

---

### Words that trigger defensiveness

The SCARF model identifies five social threat domains. Each word below triggers one or more:

| Word/phrase | SCARF threat | Why it triggers | Use instead |
| --- | --- | --- | --- |
| failure / failed | Status | Assigns blame to the person | issue, finding, gap |
| problem | Status | Puts reader on defense | observation, area, opportunity |
| wrong | Status | Judgmental | differs from expected, inconsistent with |
| broken | Status | Strong negative | not functioning as expected |
| legacy | Status | Dismissive of someone's work | established, existing |
| anti-pattern | Status | Labels past work as wrong | pattern to revisit |
| obviously / clearly | Status | Implies reader should already know | (delete — state the fact directly) |
| You always / never | Fairness | Sweeping generalization | In [specific instance]... |
| You should / need to | Autonomy | Control language | One approach is..., Consider... |
| however / but (after praise) | Certainty | Erases the preceding positive | (restructure — separate the praise) |
| Why did you...? | Status, Autonomy | Accusation disguised as inquiry | What led to...? Help me understand... |
| Per my last email | Relatedness | Passive-aggressive distancing | Following up on [topic] |
| "Some people on the team" | Relatedness | Unnamed faction, creates paranoia | "I heard a concern about..." or name yourself |
| "I'll handle it myself" | Relatedness | Excludes the reader from collaboration | "Let me take a first pass, then I'd like your input" |
| "We'll see" / "TBD" | Certainty | Leaves the reader in limbo | "I'll have an answer by [date]" |
| "Things are changing" | Certainty | Vague threat to stability | Name the specific change and timeline |
| "Going forward" (without specifics) | Certainty | Implies new rules without stating them | State the specific new expectation |

---

### Blame-to-learning patterns

| Blame pattern | Learning pattern |
| --- | --- |
| "You failed to..." | "The process didn't catch..." |
| "This is wrong" | "Here's how we can improve..." |
| "Who approved this?" | "What can we change to prevent..." |
| "Obviously..." | "One approach is..." |
| "I don't understand why..." | "Help me understand..." |
| "You should have..." | "Next time we could..." |
| "That was a bad decision" | "The decision didn't account for [factor]" |
| "They dropped the ball" | "The handoff process didn't have a checkpoint" |
| "It was a miscommunication" | "The communication path between [A] and [B] didn't surface [fact]" |
| "That's not my job" | "The responsibility boundary wasn't clear" |

---

### Non-apology patterns

| Non-apology | Why it fails | Genuine version |
| --- | --- | --- |
| "Sorry if that caused inconvenience" | Conditional — doubts harm occurred | "I missed the deadline and that delayed your work" |
| "Mistakes were made" | Passive voice — no ownership | "I made a mistake" |
| "That's just how I am" | Dismisses impact as personality | "I see how that landed and I'll change my approach" |
| "I'm sorry you feel that way" | Centers the reader's reaction as the problem | "I'm sorry I said that. It was unfair" |
| "We apologize for any inconvenience" | Vague corporate boilerplate, doubts specific harm | "We lost your data between 2pm and 4pm. Here's what we're doing" |
| "We take this very seriously" | Tells instead of shows | Describe the specific action taken |

---

### Passive-aggressive phrases

| Phrase | Subtext | Direct alternative |
| --- | --- | --- |
| "Per my last email" | You didn't read it | "Following up on [topic]" |
| "For future reference" | You did it wrong | "What about trying X instead?" |
| "As previously discussed" | I'm annoyed at repeating myself | "To confirm what we agreed on..." |
| "I've copied [manager]" | I'm escalating you | "I'd like to work together on this" |
| "Just to be clear" | You're confused and I'm not | "To make sure we're aligned..." |
| "Friendly reminder" | This is not friendly | "Following up — deadline is [date]" |
| "With all due respect" | I'm about to be disrespectful | (Delete — just state your point) |
| "No worries" (when there clearly are) | Dismissing valid frustration | "I understand that was frustrating" |
| "I'm sure you're busy, but..." | Guilt trip | "When you have time, could you..." |

---

## The two-prompt anti-AI audit

After completing all pattern fixes (AI patterns 1-24 and professional communication patterns 25-32), run this self-check:

**Prompt 1:** "What makes the below so obviously AI-generated?"
Answer briefly with remaining tells -- look for rhythm uniformity, residual vocabulary, missing personality, and structural symmetry.

**Prompt 2:** "Now make it not obviously AI-generated."
Revise to fix the remaining tells. This second pass often catches rhythm issues and soullessness that survived the pattern sweep.

---

## Quick-reference: what detection tools actually measure

| Metric | What it captures | Human profile | AI profile |
|---|---|---|---|
| Perplexity | How surprising word choices are | High -- unpredictable, idiosyncratic | Low -- safe, statistically probable |
| Burstiness | Sentence length variation | High -- wild oscillation | Low -- narrow 15-25 word band |
| Stylometric entropy | Lexical variety | High -- unique word usage | Low -- repetitive phrasing |

Key finding: as models get more fluent, they become *more* distinguishable because their consistency is even more uniform. Smoothness itself is the tell.

---

## Reference

This catalog is based on [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), maintained by WikiProject AI Cleanup, combined with research from:
- "Delving into LLM-Assisted Writing" (Science Advances, 2024)
- GPTZero AI Vocabulary analysis (3.3M texts)
- Northeastern University syntactic template studies
- University College Cork literary stylometry (2025)
