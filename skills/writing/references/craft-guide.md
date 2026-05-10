# Craft Guide: Structure, Voice, and Genre Templates

Deep reference for writing from scratch, structural revision, and voice development. Drawn from King, Zinsser, Handley, Saunders, Graham, and McCormick.

---

## How the best writers structure their work

### Paul Graham -- The conversational essayist

Every essay organized around a single pithy thesis guessable from the title. His distinguishing move: coupling abstract concepts with concrete examples. ~70% of essays contain "for example" and a specific illustration is never more than a sentence behind any abstract claim.

His sentences mirror conversation: short ones as pauses for emphasis, longer ones carry analytical momentum.

**Graham's process:** Loose then tight. Write a fast exploratory draft trying all kinds of ideas. Then spend days rewriting -- reading sentences dozens of times, abandoning whole branches that don't serve the core thesis.

**Graham's formula for useful writing:** correctness x importance x novelty x strength. A zero in any one makes the product zero. The "strength" axis is where AI-assisted writing collapses.

### Lenny Rachitsky -- The tactical operator

Deeply researched, no-nonsense tactical content. 10-100+ hours per post. Structure follows Situation-Complication-Resolution (Minto Pyramid).

Opens with a blunt insight or surprising data point. Sets brief context. Delivers tactical breakdown with specific frameworks, named companies, real numbers. Tone reads like a smart operator writing directly to a peer -- casual, fluff-free, honest about what he doesn't know.

### Packy McCormick -- The unexpected hook

Opens Not Boring essays with something seemingly unrelated to the actual topic. Readers get three-quarters through before realizing they're learning the real subject.

**Structural signature:** the "breathing room" pattern. After every dense analytical section, insert a meme, joke, or one-line paragraph that functions like breath in speech. This is why his 10,000-word essays feel shorter than a typical 2,000-word blog.

Alternating layers of graphics, analysis, lists, and quotes -- a mosaic of element types that keeps the eye engaged.

### The universal pattern

Open with a question the reader wants answered. Alternate between density and relief. Couple every abstraction with a specific example. Edit with extreme prejudice. None of them write in a single pass. All prioritize their own curiosity over what they think the audience wants.

---

## Writing masters: core principles

### Stephen King (On Writing)

- The adverb is not your friend. "He slammed the door" not "he closed the door firmly."
- Second draft = first draft minus 10%.
- Write with the door closed (first draft for you). Rewrite with the door open (second draft for the reader).
- Read a lot. Write a lot. There is no shortcut.

### William Zinsser (On Writing Well)

- Clutter is the disease of American writing. "Assistance" -> help. "Numerous" -> many. "Facilitate" -> ease.
- Strip every sentence to its cleanest components.
- Unity: every piece should be consistent in pronoun, tense, and mood.
- The secret of good writing is to strip every sentence to its cleanest components.
- Sometimes cut 50%.

### Ann Handley (Everybody Writes)

- Start with the Ugly First Draft (UFD). Get thoughts on paper without pressure.
- Write as if talking to one person.
- Present tense default: "he walks" not "he was walking."
- Count your "you" and "I" -- prioritize addressing the reader.
- Read aloud. Where you stumble is where the writing fails.
- Be "rabid about readability."
- Empathy for the reader should be at the root of all content.

**Handley's humanizing techniques:**
- Metaphors as insider winks (use language that reflects the audience's specific context)
- Go hard on a theme to create a specific mood
- The reader cameo: address the reader's internal skepticism directly
- Engage multiple senses (not just visual)
- Intentional word choice: unusual or specific words act as "hand grenades" signaling personality

### George Saunders (A Swim in a Pond in the Rain)

- Follow your "micro-opinions" -- small visceral reactions of pleasure or irritation during revision.
- Authentic voice comes from embracing your natural way of speech, not imitating an erudite voice that isn't yours.
- "Wonkiness" -- the inherent flaws and idiosyncrasies of the narrator -- is what makes prose feel true.
- Every sentence must earn its place by connecting causally to what came before.
- Matt Stone/Trey Parker rule: replace "and then" with "therefore" or "but." If a sentence only connects with "and then," it doesn't belong.

---

## Genre templates

### Blog post (technical / evangelism)

```
1. Problem snapshot    -> the moment it bites (specific incident)
2. Thesis / promise    -> "Stop doing X. Do Y instead."
3. 3 moves (ranked)    -> not a laundry list -- prioritized
4. Example per move    -> before/after, snippet, screenshot, metric
5. Tradeoffs           -> "This fails when..."
6. Decision rule       -> "If you see ___, choose ___."
```

The opening should be the problem, not the solution. Don't start by defining terms or giving history. Start with the moment something breaks, confuses, or costs money.

**Pre-flight checklist:**
- [ ] Opens with a problem, not a definition or history
- [ ] Thesis is debatable (someone could disagree)
- [ ] 3+ concrete anchors (numbers, proper nouns, failure modes)
- [ ] Each move is ranked, not just listed
- [ ] Tradeoffs section is honest, not a disclaimer
- [ ] Reader can act on the decision rule

### Newsletter

```
1. Lead                -> "One thing I noticed this week..." (personal, brief)
2. The point           -> 1 paragraph
3. Proof               -> 1 example + 1 link
4. Closer              -> "If you try one thing, try this: ___."
```

One primary idea per issue. Everything else supports it. The letter is more important than the news -- consistent voice and curation is what separates a newsletter from a feed.

Repeatable segments help: "One thing I changed," "One link worth your time," "The tool I couldn't stop using."

**Pre-flight checklist:**
- [ ] One primary idea (not three)
- [ ] Personal lead (not a news summary)
- [ ] Proof is one specific example, not a list
- [ ] Closer gives one actionable takeaway
- [ ] Voice is consistent with prior issues

### Editorial / op-ed

```
1. Hook                -> surprising fact or specific scene
2. Nut graph           -> one-sentence stance
3. 3 supports          -> each with evidence
4. Concession          -> strongest counterargument, addressed honestly
5. Action              -> what should change tomorrow
```

The concession is mandatory. Writing the best opposing point in one sentence and then rebutting with one fact + one principle is what separates advocacy from propaganda. AI skips this or fakes it.

**Pre-flight checklist:**
- [ ] Stance is clear in the first 10%
- [ ] Each support has specific evidence (not just argument)
- [ ] Concession addresses the strongest counterargument, not a strawman
- [ ] Action is specific — what should change tomorrow
- [ ] Reader could disagree with your position (it's not a truism)

### Internal evangelism doc

```
1. The problem I saw   -> specific incident, team, system
2. What I tried        -> tool/technique with real output
3. What broke          -> honest failure mode
4. What worked         -> measurable result
5. How to steal this   -> 3 steps someone can take Monday morning
```

Structured like a trip report, not a policy document. Show the command output. Name the tool version. Include the error message. This is unfakeable context.

**Pre-flight checklist:**
- [ ] Problem is a specific incident, not an abstract category
- [ ] "What I tried" includes real output (commands, screenshots, metrics)
- [ ] "What broke" is honest — not glossed over
- [ ] "What worked" has a measurable result
- [ ] "How to steal this" has 3 steps someone can take Monday morning

### Analytical briefing / white paper

The analytical briefing is the genre that blog posts and evangelism docs cannot do: structured analysis of a technical event, trend, or system, written for enterprise decision-makers who need to understand what happened, why it matters, and what to do about it. Authority comes from evidence curation, not personal voice.

**Structure:**
```
1. Executive framing      -> What happened + why it matters (2-3 sentences, no preamble)
2. Background             -> Just enough context for the reader to follow the analysis
3. What was found         -> Technical findings, each with cited evidence
4. "So what" translation  -> Each finding mapped to organizational implications
5. Recommendations        -> Concrete, scoped to specific teams or functions
6. Visual synthesis       -> Summary diagram connecting findings to actions
```

**The "so what" translation pattern:** This is the spine of an analytical briefing. Every technical finding must be immediately followed by its organizational implication. The pattern has three layers:

1. **Finding:** What the evidence shows (technical, specific, cited)
2. **General significance:** Why this matters beyond the specific event
3. **Organizational implication:** What this means for *the reader's organization* specifically

Example: "The leaked code confirmed that Claude Code runs multiple AI worker processes in parallel [REF-111]." → "This keeps the main agent's working memory from filling up with intermediate results." → "This is directly relevant to Walmart because Wibey uses the Claude Agent SDK. The scaffolding patterns the leak exposed are the same mechanisms that govern Wibey's behavior."

Without the third layer, the paper is a literature review. With it, it is a briefing.

**Declarative section titles:** Use section titles that state findings or questions, not category labels. "How the Agent Remembers Project Context" tells the reader what they will learn. "Memory Architecture" tells them what topic they are entering. The former carries the argument; the latter just organizes it.

**Measured authority voice:** The analytical briefing takes strong positions — but attributes them to evidence rather than to the author's opinion. "The most important finding from the community's analysis: agent quality depends on the scaffolding" is authoritative because it cites a source, not because the author asserts it. This is evidence-attributed confidence: the paper makes claims the reader can verify rather than claims the reader must take on faith.

Rules for the analytical register:
- Third person throughout. No "I" or "we" unless quoting.
- No contractions. Measured cadence signals authority.
- No fragments, asides, or register shifts. Structure is the texture.
- Active voice for findings ("The leak exposed..."), passive only when the actor is genuinely unknown.
- Strategic sentence variation: not the wild burstiness of a blog, but deliberate shifts between short declarative sentences and longer analytical ones.

**Citation architecture:** Analytical briefings need a systematic reference approach, not just inline anchors. Choose a format (numbered references, author-date, or tagged references like `[REF-1]`) and use it consistently. References should accumulate across sections — by the third section, the reader has seen enough cited evidence to trust the analysis. Cross-reference between sections when findings build on each other.

**Diagram placement:** Deploy diagrams at three natural points: (1) after explaining a complex system or architecture, as visual summary; (2) at structural transitions between major sections, as breathing room (the McCormick "breathing room" pattern); (3) at the end, as a full argument map connecting findings to recommendations. Keep diagrams minimal — labels and arrows, not comprehensive data visualizations. Each diagram should be readable in 10 seconds.

**Common mistakes:**
- Writing a literature review instead of a briefing (findings without "so what")
- Using blog-post voice in an analytical piece (contractions, first person, asides)
- Category-label section titles ("Background," "Analysis," "Recommendations") instead of declarative titles
- Synonym cycling key terms instead of repeating them consistently (see craft techniques below)
- Forcing personality into a genre that earns trust through evidence, not charm
- Exhaustive coverage of every finding instead of prioritizing the ones that matter most
- Burying recommendations at the end without connecting them back to specific findings
- Diagrams that decorate rather than synthesize

**Pre-flight checklist:**
- [ ] Executive framing in the first 2-3 sentences — no preamble
- [ ] Every finding is cited with a consistent reference format
- [ ] Every finding has a "so what" — organizational implication stated explicitly
- [ ] Section titles are declarative claims or questions, not category labels
- [ ] Third person throughout (no "I" or "we" except in quotes)
- [ ] No contractions; formal register is consistent
- [ ] Key terms are established once and reused consistently, not cycled through synonyms
- [ ] Named-source quotes are integrated with attribution + role + verb + quote pattern
- [ ] Recommendations are scoped to specific teams or functions, not generic
- [ ] At least one diagram synthesizes findings visually
- [ ] A closing summary connects findings to actions (visual or textual)
- [ ] The piece would survive having the author's name removed — authority comes from evidence, not persona

---

## High-stakes communication templates

These genres are harder than blog posts because written tone lacks body language and vocal cues. Readers re-read emails, re-interpret intent, and share them with others. The templates below over-invest in tone markers — acknowledgment, forward-looking language, explicit care — because the medium strips those signals away.

Each template includes a structure, common mistakes, and a pre-flight checklist. For interpersonal pattern checks, see `references/ai-pattern-catalog.md` patterns 25-29.

### Decline email

**Structure (target: 50-125 words for peak response rate; keep under 200 — Boomerang 2016, 40M emails):**
```
1. Specific acknowledgment  -> Name something concrete from their work
2. Decision                 -> Don't bury it. First or second paragraph
3. 2-3 honest reasons       -> Framed as YOUR requirements, not their gaps
4. Genuine specific compliment -> Something only someone who engaged would notice
5. Personal closer          -> A specific action that proves engagement
```

**Tone:** Respectful peer closing a door honestly. You're explaining what you need, not what they lack.

**Common mistakes:**
- Burying the "no" in paragraph four (readers decode your hedging as dishonesty)
- Implying follow-up that never happened ("questions we couldn't resolve")
- Framing that invalidates their effort ("we're solving this internally")
- Generic warm closers ("we wish you the best")
- Over-explaining the evaluation process or revealing comparative vendor info

**Pre-flight checklist:**
- [ ] Did you actually do what your framing implies?
- [ ] Does any reason make the reader's effort sound pointless?
- [ ] Are your reasons observations or inferences?
- [ ] Does your compliment name something specific?
- [ ] Does your closer include a personal action, not just a wish?
- [ ] Decision in the first or second paragraph?
- [ ] Under 200 words?

### Incident report / postmortem

**Structure:**
```
1. Summary             -> 2-3 sentences: what happened
2. Impact              -> Quantified: duration, affected users, business cost
3. Contributing factors -> Systems, not people. Plural — never a single root cause
4. Timeline            -> Chronological with timestamps. Start BEFORE the incident
5. What went well      -> Detection speed, response quality, communication
6. What went wrong     -> Process gaps, tooling failures, visibility issues
7. Where we got lucky  -> Hidden risks that didn't bite this time
8. Action items        -> Owner + ticket + priority. Bounded, specific, completable
```

**Tone:** Neutral narrator focused on systems. "What happened" not "who did it."

**Blameless language rules:**
- Ask "what" and "how" questions, not "why" and "who"
- No individual's action is a root cause — describe the system that allowed it
- No counterfactuals ("should have," "could have") — these describe fictional realities
- Frame improvements as systemic: "the process didn't catch" not "you failed to"

**Common mistakes:**
- Treating human error as root cause instead of symptom
- Punishment framing that discourages future knowledge sharing
- Vague action items ("make the system faster") instead of bounded tasks
- Skipping "where we got lucky" — this surfaces hidden risk
- Using "outage" when the actual impact was partial degradation

**Pre-flight checklist:**
- [ ] No individual named as a cause or blamed
- [ ] Contributing factors are systemic, not personal
- [ ] Timeline starts before the incident (avoids hindsight bias)
- [ ] Impact is quantified with real numbers
- [ ] Action items have an owner, ticket, and priority
- [ ] "What went well" section is present and genuine
- [ ] "Where we got lucky" section is present
- [ ] All claims pass the Camera Test

### Written feedback

**Structure (SBI model):**
```
1. Situation     -> Specific date and context: "During Tuesday's sprint review..."
2. Behavior      -> Observable action a camera could record. Not traits, not motives
3. Impact        -> Consequence or your personal response: "The team lost the thread"
4. Intent inquiry -> "What were you hoping to accomplish?" (closes the assumption gap)
```

**Tone:** Caring colleague with specific observations. Describe the verb, not the adjective. The art critique ladder applies: Describe what you see -> Analyze how it works -> Interpret what it means -> Evaluate how it lands.

**Radical Candor HHIPP for written feedback:**
- **Humble** — your perspective has limits
- **Helpful** — framed for growth, not punishment
- **Immediate** — address promptly
- **In-person-equivalent directness** — be as direct as you would face-to-face
- **Don't Personalize** — critique the work, not the person's character

**Common mistakes:**
- Inserting judgments: "You were difficult" vs. "You rejected three proposals without offering alternatives"
- Vague timeframes: "recently" vs. "during Tuesday's standup"
- Assuming intent without asking
- Falling into Ruinous Empathy — softening until the message disappears
- Delivering serious feedback for the first time in writing (use a conversation first)

**Pre-flight checklist:**
- [ ] Situation is specific (date, meeting, context)
- [ ] Behavior is observable (Camera Test passes)
- [ ] Impact is concrete (business outcome, team effect, or personal response)
- [ ] No character judgments — only behavior descriptions
- [ ] Intent inquiry included or follow-up conversation offered
- [ ] Sent privately, not to a group

### Escalation email

**Structure:**
```
1. Issue statement       -> Facts, not emotions. Specific details
2. Prior attempts        -> With dates. Builds credibility, shows good faith
3. Impact               -> What's blocked, delayed, or at risk
4. Specific ask          -> A decision, prioritization, or action — with a deadline
```

**Tone:** Collaborative problem-solver with receipts. Assume the reader wants to help and needs clarity. Not a performance critique — a request to unblock work.

**Common mistakes:**
- Escalating too early (appears impatient) or too late (forces rushed decisions)
- Over-CCing — trains people to ignore your escalations
- Burying the ask so the reader has to hunt for it
- Framing as a warning rather than a request for support
- Surprise escalations — give people a chance to resolve first

**Pre-flight checklist:**
- [ ] Issue meets a clear threshold for escalation (not just frustration)
- [ ] 1-2 prior follow-up attempts documented with dates
- [ ] Tone is factual, not emotional
- [ ] Impact tied to business outcomes the reader cares about
- [ ] Ask is specific and actionable with a deadline
- [ ] Recipients chosen for decision authority, not pressure
- [ ] No surprise — affected parties had a chance to resolve first

### Apology email

**Structure:**
```
1. Name the harm      -> Specific, not vague. "I missed the deadline" not "sorry for any issues"
2. Brief explanation   -> Context, not excuse. 1-2 sentences max
3. Own it             -> "I" + active voice. Not "mistakes were made"
4. Corrective action   -> What you're doing to fix the immediate damage
5. Prevention         -> What changes to prevent recurrence
```

**Tone:** Direct owner taking responsibility without deflection. Words mean more when preceded by action — apologize after demonstrating you understand the harm.

**Genuine vs. non-apology:**
- "I" and active voice = genuine. "We" and passive voice = evasive
- "I missed the deadline" = genuine. "Sorry if the timing caused inconvenience" = non-apology
- Naming specific harm = genuine. "Sorry for any issues" = non-apology
- See `references/ai-pattern-catalog.md` non-apology patterns table for the full list

**Common mistakes:**
- Burying the apology in justification
- Using "sorry" as a verbal tic without specificity
- Conditional language: "sorry if," "sorry but"
- Omitting what changes going forward (apology without prevention is just PR)
- Centering your own discomfort: "this has been hard for me too"
- Delaying — speed signals sincerity. Same-day reads as genuine; a week later reads as damage control

**Pre-flight checklist:**
- [ ] Specific harm named (not vague regret)
- [ ] "I" language, active voice (not passive, not conditional)
- [ ] No "sorry if" or "sorry but" constructions
- [ ] Explanation is brief and does not function as an excuse
- [ ] Concrete corrective action described
- [ ] Prevention measures outlined
- [ ] Sent within 24 hours of recognizing the error
- [ ] No defensive or minimizing language

### Status update / executive summary

**Structure:**
```
1. Bottom line up front (BLUF) -> The one thing the reader must know
2. Progress since last update   -> 2-3 bullet points, measurable where possible
3. Risks and blockers           -> Don't bury bad news. State it after progress
4. Help needed                  -> Specific asks, not vague "any support welcome"
5. Next milestones              -> What's coming, with dates
```

**Tone:** Competent operator reporting to someone with less context and less time. Assume 30 seconds of attention.

**Common mistakes:**
- Burying risk behind good news (the reader remembers you hid it)
- No clear ask (if you need something, say so — don't hint)
- Wrong detail level for the audience (exec wants outcomes, not implementation details)
- Activity reporting instead of progress reporting ("we did X" vs. "X is now at Y%")
- Symmetric coverage of all workstreams when one is the only thing that matters

**Pre-flight checklist:**
- [ ] Bottom line is in the first sentence
- [ ] Risks are stated, not hidden
- [ ] Asks are specific and actionable
- [ ] Detail level matches the audience
- [ ] Progress is measured, not described ("shipped" not "worked on")

### Customer complaint response

**Structure:**
```
1. Acknowledge          -> Name their specific experience, not a generic category
2. Own what's yours     -> Even if the cause is ambiguous, own the impact
3. Explain (briefly)    -> What happened, not why it's not your fault
4. Resolution           -> What you're doing to fix THIS instance
5. Prevention           -> What changes to prevent recurrence
6. Invitation           -> Make it easy to follow up if it's not resolved
```

**Tone:** Calm professional who cares about the outcome, not defensive representative protecting the brand. You may not be at fault, but the reader is unhappy and that's real.

**Common mistakes:**
- Leading with policy instead of empathy ("Our terms state...")
- Explaining before acknowledging (reader hears "excuses" before "I hear you")
- Conditional ownership: "We're sorry if..." vs. "We're sorry this happened"
- Closing without a specific resolution or next step
- Corporate boilerplate that could apply to any complaint

**Pre-flight checklist:**
- [ ] Specific experience acknowledged (not "your recent issue")
- [ ] Impact owned regardless of fault determination
- [ ] Explanation is brief and factual, not defensive
- [ ] Resolution is concrete and specific to this case
- [ ] Follow-up path is clear and easy
- [ ] No corporate boilerplate ("we value your business")

### Recommendation / endorsement letter

**Structure:**
```
1. Relationship context  -> How you know them, how long, in what capacity
2. Specific claim        -> ONE thing that makes them exceptional (not five vague things)
3. Evidence              -> A specific story, project, or result that proves the claim
4. Comparison context    -> How they stand out relative to peers (without naming peers)
5. Unqualified endorsement -> Direct statement with no hedging
```

**Tone:** Advocate with specific evidence. You're not describing a person — you're making an argument that a decision-maker should act on.

**Common mistakes:**
- Vague praise: "great team player," "hardworking," "pleasure to work with" — could describe anyone
- Listing five qualities instead of proving one deeply
- No specific story or result (the letter has no memory of a real person)
- Hedging the endorsement: "I believe they would be a good fit" vs. "Hire them"
- Writing generically enough that swapping the name would still work

**Pre-flight checklist:**
- [ ] Relationship context is specific (role, duration, capacity)
- [ ] ONE exceptional quality is named and argued, not five listed
- [ ] A specific story or result proves the claim
- [ ] Endorsement is unhedged and direct
- [ ] Swapping the name would break the letter (it's that specific)

---

## When NOT to write

Writing is the wrong medium when:
- **Serious feedback for the first time.** Have a conversation first. Written feedback is for follow-up, documentation, or minor issues — not for the first time someone hears something difficult.
- **Emotional complexity requires tone.** If the reader's reaction depends on hearing your voice, seeing your face, or reading your body language, a meeting or call is better.
- **Real-time dialogue is needed.** If you expect questions, pushback, or negotiation, writing forces a slow async loop that frustrates both parties.
- **The stakes justify the bandwidth.** Termination, major performance issues, sensitive organizational changes — these deserve synchronous human presence.

When in doubt: would you want to receive this message in writing, or in person?

---

## Subject lines and titles

Subject lines determine whether your email gets opened, read first, or triaged to "later" (which often means never).

**Email subject line principles:**
- Lead with the action or decision needed: "Decision needed: vendor selection by Friday"
- Include the topic and urgency: "[Escalation] API latency — blocking release"
- For status updates, lead with the bottom line: "Project Alpha: on track, one risk"
- Never use vague subjects: "Quick question," "Following up," "FYI"
- Match the subject to the email's actual content — if the subject says "update" but the email asks for a decision, the subject is wrong

**Blog/article title principles:**
- The thesis should be guessable from the title (Graham)
- Specific beats generic: "Why we switched from Redis to DragonflyDB" > "Choosing a cache"
- Promise a benefit or provoke curiosity, not both
- If the title works for 1,000 different articles, it's too vague

---

## Audience calibration

The same message needs different framing for different readers. Adjust three dimensions:

| Dimension | Peer / IC | Leadership / exec | Cross-functional |
| --- | --- | --- | --- |
| **Detail level** | Implementation specifics, code, configs | Outcomes, metrics, business impact | Context + why it matters to them |
| **Vocabulary** | Domain jargon is fine | Translate jargon to business terms | Define terms or use plain language |
| **Ask framing** | "Can you review this PR?" | "I need a decision on X by Y" | "Here's how this affects your team" |
| **Length** | As long as needed | Short — assume 30 seconds of attention | Medium — enough context to orient |

**The upward-communication trap:** When writing to leadership, the instinct is to show your work. Resist it. Executives want the conclusion, the risk, and the ask. The evidence is there if they ask for it — not front-loaded by default.

**The cross-functional trap:** When writing to another team, the instinct is to explain your domain. Instead, explain the *impact on their domain*. "Our API change means your integration tests will break on Tuesday" is better than "We're refactoring the auth middleware."

---

## Craft techniques for analytical writing

These techniques apply primarily to analytical genres (briefings, white papers, technical evaluations) but elements are useful across all writing.

### Strategic term repetition

The inverse of synonym cycling (pattern 11 in `ai-pattern-catalog.md`). In analytical writing, repeating a key term *is the point* — it signals precision, not laziness.

The pattern: establish a term with a clear definition early in the piece, then reuse that exact term throughout. Do not cycle through synonyms. If you write "scaffolding" to mean "the code wrapped around an AI model," use "scaffolding" every time. Do not alternate with "framework," "harness," "wrapper," or "infrastructure" — each introduces ambiguity about whether you mean the same thing.

**When to repeat:** Technical concepts that carry specific meaning in the paper's argument. "Scaffolding," "working memory," "feature flags," "citation architecture."

**When NOT to repeat:** Common verbs and connectors. If every paragraph opens with "The paper" or "The analysis," that is monotony, not precision. Vary the *vehicle* (sentence structure, subject position) while keeping the *cargo* (the technical term) stable.

### Named-source quote integration

When a piece cites specific people, integrate their words using this pattern: **attribution + role + verb + quote + context**.

The verb carries epistemic weight:
- **observed** — neutral, descriptive
- **argued** — takes a position
- **noted** — factual, low-stakes
- **identified** — analytic, structural
- **warned** — introduces risk
- **confirmed** — adds corroboration

**Before:** Industry experts say the leak was significant.

**After:** Joshua Sum, CEO of Solayer, observed that the leak "shaved a year of reverse-engineering off every startup and enterprise's roadmap."

The role gives the reader a reason to trust the quote. The verb tells the reader how to weight it. The quote provides the specificity. Do not paraphrase when the source's exact words are more precise or vivid than your summary would be.

### Diagram placement as rhetorical architecture

Diagrams in analytical writing serve three rhetorical functions, not just information design:

1. **Visual summary** — after a dense analytical section, a diagram distills what was just explained into a scannable form. Place these immediately after the text they summarize, not before.

2. **Structural breathing room** — between major sections, a diagram provides the "breathing room" that Packy McCormick uses with memes and one-liners in long-form essays. Dense analysis + diagram + dense analysis is easier to read than three consecutive blocks of dense analysis.

3. **Argument map** — at the end, a diagram connecting findings to recommendations gives the reader a single image that captures the paper's entire argument. This is the most valuable diagram in the piece and should be the last visual element.

**Rules:**
- Diagrams should be minimal: labels and arrows, readable in 10 seconds
- Do not create diagrams that try to be comprehensive — they should synthesize, not catalog
- One diagram per major section is the maximum; most pieces need 2-3 total
- If a diagram requires a paragraph of explanation to make sense, it has failed

---

## Voice development framework

### Building a voice spec from writing samples

If the user provides 3-5 samples of their best writing, analyze for:

1. **Sentence length distribution** -- average, range, standard deviation
2. **Transition style** -- causal ("That's why..."), abrupt (new paragraph, no connector), conversational ("So here's the thing...")
3. **Metaphor/analogy frequency and source domain** -- technical? physical? pop culture?
4. **Formality level** -- contractions, slang, jargon, register shifts
5. **Signature phrases** -- recurring patterns, pet constructions
6. **Structural patterns** -- how they open, how they close, how long their paragraphs run
7. **Stance style** -- how they express opinions (directly? through examples? through questions?)

Codify these into voice rules. Use them as constraints for all future writing and editing.

### Default voice rules (when no samples provided)

**Personal-voice genres (blog, newsletter, evangelism, comms):**
- Contractions always
- Active voice dominant
- First person when appropriate
- At least one real-world example per section
- At least one position taken without hedging per piece
- No kill-list vocabulary
- No template transitions
- Causal connectors over additive ones

**Analytical genres (briefing, white paper, policy analysis):**
- No contractions; formal register throughout
- Third person exclusively (no "I" or "we" except in quotes)
- Active voice for findings; passive only when actor is unknown
- Positions through evidence attribution, not personal opinion
- Key terms established once and reused, not cycled
- Named-source quotes with attribution + role + verb pattern
- No kill-list vocabulary
- No template transitions
- Measured cadence: deliberate variation, not wild burstiness

### Tone spectrum by context

| Context | Tone |
|---|---|
| Blog post | Opinionated practitioner teaching a peer |
| Internal evangelism | Trip report from someone who did the thing |
| Newsletter | Smart friend sharing one thing they learned |
| Technical doc | Precise, clinical, but still first-person |
| Slack / internal comms | Casual, punchy, meme-literate |
| Analytical briefing | Evidence-attributed analyst presenting findings to decision-makers |
| Decline email | Respectful peer closing a door honestly |
| Incident report | Neutral narrator focused on systems, not people |
| Written feedback | Caring colleague with specific observations |
| Escalation | Collaborative problem-solver with receipts |
| Apology | Direct owner taking responsibility without deflection |

---

## The science behind human vs. AI writing

### Why this matters for craft

Detection tools measure the same qualities writing teachers have always advocated. Sentence variation isn't just aesthetically pleasing -- it's a measurable signature of human authorship.

### Perplexity

Measures how surprising word choices are. AI text has low perplexity (selects the most statistically probable next word). Human text has high perplexity (unusual verbs, inventive metaphors, personal references).

### Burstiness

Measures sentence length variation. AI: narrow band of 15-25 words. Humans: wild oscillation from 3-word fragments to 40-word complex sentences.

### The smoothness paradox

As GPT-4 produces more fluent text than GPT-3.5, it becomes *more* distinguishable in stylometric analysis because its consistency is even more uniform. The machine gets smoother, and smoothness itself becomes the tell.

### The biological basis

Human speech pulses at ~1.6 seconds per intonation unit across 48 languages, aligned with low-frequency brain activity linked to memory and attention. Prose that varies cadence to match these biological rhythms resonates with the reader's cognitive processing. Uniform cadence feels wrong at a level below conscious awareness.

### Attribution bias

When readers believe a text was written by a human, they find it more credible, effective, and trustworthy than identical text attributed to AI. The human fingerprint is perceived as a quality marker even by AI models evaluating text.

---

## The AI-as-brainstorm-partner workflow

The most recommended approach for maintaining authentic voice when using AI assistance:

1. **You** write the outline based on your actual experience and knowledge
2. **You** write the opening -- a personal anecdote, a specific incident, a hook grounded in something only you witnessed
3. **AI** drafts middle sections from your detailed bullet points
4. **You** rewrite every AI paragraph in your voice, adding specifics, opinions, and personality
5. **You** write the conclusion -- your opinion, your call to action
6. **Run the six-pass edit** from the main SKILL.md
7. **Read aloud**, purge AI-isms, verify facts

### The style guide training approach (Tiago Forte method)

1. Gather 3-5 pieces that represent your best writing
2. Feed them to AI with instructions to generate an elaborate style guide covering voice, tone, sentence structure, transition style, rhythm, and signature patterns
3. Save the resulting guide as a system prompt for all future drafts
4. The analysis improves with each additional sample

---

## Key sources

- King, Stephen. *On Writing.*
- Zinsser, William. *On Writing Well.*
- Handley, Ann. *Everybody Writes.*
- Saunders, George. *A Swim in a Pond in the Rain.*
- Graham, Paul. "How to Write Usefully." paulgraham.com
- Fishbein, Ellen. "What Makes Paul Graham a Great Writer?" ellenrhymes.com
- "Un-Packy-ng Technical Writing." newsletter.artofscience.com
- Forte, Tiago. "How to Create an AI Style Guide." fortelabs.com
- Wikipedia. "Signs of AI writing." WikiProject AI Cleanup.
