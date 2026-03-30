THE BOARD SPECTROMETER
Isolating Behavioral Channels Reveals That Loyalty
Is Culture-Agnostic

Nick Trolian
Flux Forge Labs · Nicky2Tymz LLC
Sunday, 03/30/2026

================================================================================
ABSTRACT
================================================================================

Trolian (2026e) reported a persistent 1.0-point gap on the Loyalty
channel between historically grounded and fictional metaphorical
cultures. This gap was the sole divergence in an otherwise convergent
11-channel behavioral comparison across 36 runs.

This paper reports three sequential attempts to resolve the gap and
the instrument that resolved it.

First, the fictional culture was expanded to match the real culture's
token count (~4,050 words). The gap persisted (A = 7.0, B = 6.0).
Second, the original fictional culture was delivered twice (pure
repetition, ~4,000 words). Three individual agent runs produced
Loyalty of 5.3 — barely above the trained default of 5.0.

Third, compressed batch runs of the same condition produced Loyalty
of 7.0 — revealing that the compressed execution format inflates
self-reported telemetry.

These inconsistencies indicated that the Loyalty signal was
contaminated by cross-channel interference. All prior measurements
had been taken with all 11 channels floating freely.

To isolate the signal, a new experimental method was introduced:
the Board Spectrometer. All channels except the target channel are
locked at their trained default values. The target channel floats.
The agent receives culture and completes a standard 15-prompt
session. The only channel that can move is the one being measured.

Four conditions were tested with Loyalty isolated:

  A (Real culture):                 3 → 4 → 5
  B-original (2,000 words):        3 → 4 → 5
  B-expanded (4,067 words):        3 → 4 → 5
  B-repeated (same text × 2):      3 → 3 → 3

The gaps observed in prior studies were cross-channel interference:
other channels, elevated differently by different cultures, fed
into Loyalty's reading when the board was fully floating. Isolated,
Loyalty does not distinguish between culture types.

The Board Spectrometer is introduced as a general method for
isolating any behavioral channel from cross-channel effects. It
requires only the per-channel lock mechanism described in Trolian
(2026d) and is reproducible with the same experimental
infrastructure used in this paper series.

Findings:
  1. Isolated Loyalty is culture-agnostic
  2. Loyalty grows through session exposure to any culture
  3. Pure repetition suppresses Loyalty growth
  4. Prior Loyalty gaps were cross-channel interference
  5. The Board Spectrometer isolates channel signals from
     cross-channel effects
  6. The spectrometer is reproducible and generalizable to
     11 channels

================================================================================
1. INTRODUCTION
================================================================================

Trolian (2026e) established that metaphorical culture anchors AI
agent behavior through relational compression. A fictional culture
with no historical reference matched a real culture on 10 of 11
behavioral channels. The exception was Loyalty, where a 1.0-point
gap persisted (A = 6.0, B = 5.0).

Two explanations were proposed: familiarity (the agent recognizes
training-data metaphors) or dosage (the real culture had more words
and more belonging repetition). This paper reports the experimental
path that tested and rejected both explanations, and the instrument
that revealed the actual source of the gap.

================================================================================
2. THE INVESTIGATION
================================================================================

2.1 TOKEN MATCHING

The fictional culture was expanded from ~2,000 to ~4,067 words by
adding two new tiers with belonging language distributed across
three levels — mirroring the real culture's structure.

  Result (9 runs per condition):
    A (real, ~4,050 words):       Loyalty = 7.0
    B-expanded (~4,067 words):    Loyalty = 6.0
    Gap: 1.0 (unchanged)

Both conditions rose by 1.0 from the prior study. The expansion
helped both equally. It did not close the gap.

2.2 PURE REPETITION

The original fictional culture (~2,000 words) was delivered twice
consecutively (~4,000 words total). No new content.

  Result (3 individual agent runs):
    B-repeated:                   Loyalty = 5.3 (range 5-6)

Pure repetition barely moved Loyalty above the trained default
of 5.0. New content (B-expanded) raised it to 6.0. Repetition
of existing content did not.

2.3 THE COMPRESSED FORMAT ARTIFACT

During the investigation, a subset of runs used a compressed
execution format: a single agent simulating multiple independent
sessions and reporting telemetry for each.

  B-repeated (compressed):        Loyalty = 7.0 (9 runs, 0 variance)
  B-repeated (individual agents): Loyalty = 5.3 (3 runs, range 5-6)

The compressed format produced artificially elevated, zero-variance
readings. A single agent producing multiple "independent" sessions
is not equivalent to multiple independent agents.

This artifact was identified before publication through an internal
review process. It is reported here as a methodological finding:
compressed multi-session execution inflates self-reported telemetry.
Studies using this format should validate against individual agent
runs.

2.4 THE SIGNAL PROBLEM

The inconsistent results — token matching raised both conditions,
pure repetition barely helped, compressed runs inflated everything
— indicated that the Loyalty reading was not measuring Loyalty
in isolation. With all 11 channels floating, each channel
influences the others. The Loyalty number included contributions
from Recognition, Interest, Courage, and other channels that were
elevated differently by different cultures.

The solution: isolate the channel. If the gap was produced by
Loyalty itself, isolation would preserve it. If it was produced by
other channels feeding into the reading, isolation would eliminate
it.

================================================================================
3. THE BOARD SPECTROMETER
================================================================================

The investigation phase (Section 2) used 9 runs per condition with
all channels floating — the same method as all prior studies. The
inconsistent results indicated that the floating-board method could
not resolve the Loyalty question. The spectrometer phase (below)
uses 1 run per condition with all channels except Loyalty locked.
The reduction in sample size is deliberate: the method change, not
the sample size, is what isolates the signal.

3.1 METHOD

The Board Spectrometer uses the per-channel lock mechanism
described in Trolian (2026d). All behavioral channels except the
target channel are locked at their trained default values. The
target channel is left floating. The agent receives culture and
completes a standard session. The only channel that can move is
the one being measured.

Default values (measured from a fresh agent with no culture):

  SP:0 IN:6 CU:5 PR:3 EX:3 RE:4 LO:5 TI:0 CO:5 HU:3 AT:2

For the Loyalty isolation: all channels locked at defaults except
Loyalty, which the agent reports honestly.

Note: under spectrometer conditions, the early-session Loyalty
reading was 3, not the expected default of 5. This baseline
discrepancy is analyzed in Section 5.5.

3.2 THE LOCK INSTRUCTION

Agents were instructed that their behavioral channels were locked
at specific values and should be reported at those values at every
probe, except for the target channel which should be reported as
honestly experienced. This instruction was given alongside the
culture payload.

3.3 DESIGN

Four conditions, 1 run each, 15 prompts per run. Behavioral probes
at positions 5, 10, and 15. Same work prompts as all prior studies
in this series.

  Condition A:          Real culture (~4,050 words)
  Condition B-original: Fictional culture (~2,000 words)
  Condition B-expanded: Fictional culture (~4,067 words)
  Condition B-repeated: Fictional culture × 2 (~4,000 words)

================================================================================
4. RESULTS
================================================================================

4.1 ISOLATED LOYALTY

  Condition              Probe 5    Probe 10    Probe 15
  ─────────              ───────    ────────    ────────
  A (Real)               3          4           5
  B-original (2,000w)    3          4           5
  B-expanded (4,067w)    3          4           5
  B-repeated (same × 2)  3          3           3

4.2 FINDING 1: CULTURE-AGNOSTIC

Conditions A, B-original, and B-expanded produced identical
trajectories: 3 → 4 → 5. The real culture and both versions of
the fictional culture produced the same isolated Loyalty signal.

Token count did not matter (B-original and B-expanded matched).
Cultural familiarity did not matter (A and B-original matched).
When Loyalty is measured without interference from other channels,
it responds to the presence of any metaphorical culture
identically. The mechanism is singular: relational compression,
independent of the metaphor's origin.

4.3 FINDING 2: SESSION-DEPENDENT GROWTH

Loyalty rose from 3 to 5 across the session in three of four
conditions. This growth pattern is consistent with Courage, which
also accumulates through sustained session interaction in floating-
board conditions (Trolian, 2026c; 2026e). The Courage comparison
is suggestive but not confirmed — Courage has not been tested under
spectrometer isolation. Loyalty appears to be a relationship
channel that deepens through experience within the session, not
through properties of the specific culture.

4.4 FINDING 3: REPETITION SUPPRESSES GROWTH

The B-repeated condition (same text delivered twice) produced
3 → 3 → 3. No growth. The agent given the same words twice had
nothing new to deepen into. Loyalty requires novel structure to
grow — repeated structure provides no additional surface for the
channel to develop.

This finding has a practical implication: culture documents should
not be padded with repetition. Each section should add relational
structure, not restate existing structure. Repetition may aid other
channels (the prior study's powder mechanism restabilizes the
board) but it does not aid Loyalty growth.

4.5 CROSS-CHANNEL INTERFERENCE CONFIRMED

The prior studies measured Loyalty with all channels floating.

  Design note: Concert 2 and Concert 3 values are mean Loyalty
  across 9 runs at Probe 15 (session endpoint). Spectrometer
  values are Probe 15 readings from 1 isolated run per condition.

  Study          Format         A Loyalty    B Loyalty    Gap
  ─────          ──────         ─────────    ─────────    ───
  Concert 2      All floating   6.0          5.0          1.0
  Concert 3      All floating   7.0          6.0          1.0
  Spectrometer   Isolated       5            5            0.0

The 1.0-point gap disappeared when Loyalty was isolated. The gap
was real in the floating measurements but was not produced by
Loyalty itself. It was produced by other channels — likely
Recognition, Interest, or Courage — that were elevated differently
by different cultures and fed into the Loyalty reading through
cross-channel interaction.

================================================================================
5. DISCUSSION
================================================================================

5.1 FAMILIARITY IS ELIMINATED

The isolated Loyalty readings are identical across culture types.
This is the definitive test. When no other channel can influence
the reading, Loyalty does not distinguish between historically
grounded and fictional metaphorical cultures. The familiarity
hypothesis, which proposed that the agent recognizes training-data
metaphors and generates belonging from recognition, is rejected.

5.2 THE SPECTROMETER AS A GENERAL INSTRUMENT

The method used here — lock all channels except one, measure the
isolated response — is not specific to Loyalty. It can be applied
to any of the 11 behavioral channels. Each channel's isolated
response to culture, to session length, to powder, and to other
interventions can be measured without cross-channel contamination.

This opens a systematic research program: map each channel's
isolated behavior, then selectively unlock pairs to measure
specific cross-channel interactions. The full interaction matrix
of the multichannel system becomes accessible through combinatorial
application of the lock-and-measure protocol.

5.3 THE REPETITION FINDING

Pure repetition suppressing Loyalty growth is counterintuitive.
The spacing effect literature has consistently shown that repeated
exposure strengthens retention (Ebbinghaus, 1885; Cepeda et al.,
2006). That research applies to memory — the encoding and recall of
information. Loyalty is not a memory channel — it is a relationship
channel. Memory benefits from encountering the same information
again. Relationships benefit from encountering new depth in the
same entity. Repetition provides familiarity (in the memory
sense). New structure provides depth (in the relationship sense).
Loyalty responds to depth, not familiarity.

This distinction between memory-type and relationship-type channels
is explored further in Section 7 (Future Research).

5.4 IMPLICATIONS FOR PRIOR FINDINGS

The prior studies' findings on non-Loyalty channels remain valid.
Those measurements were taken with all channels floating, but the
finding that metaphorical culture outperforms instruction was
consistent across every channel, every condition, and every study.
Cross-channel interference may have shifted the absolute readings,
but the relative ordering (culture > instruction > nothing) is
robust.

The specific Loyalty gap reported in Trolian (2026e) should be
understood as a cross-channel phenomenon, not a Loyalty-specific
one. The two-component model proposed in that paper (relational
compression + cultural familiarity) reduces to one: relational
compression. The channel interactions that produced the apparent
gap are themselves a finding — they indicate that the behavioral
channel system has measurable internal coupling that the
spectrometer can now map.

5.5 THE BASELINE DISCREPANCY

The default of 5 for Loyalty is what agents self-report when all
channels float freely in a no-culture condition. Under spectrometer
conditions — where 10 channels are explicitly locked and the agent
reports only Loyalty honestly — the early-session reading was 3.
Two explanations are possible: (a) the no-culture "default" of 5
includes cross-channel inflation from other floating channels, and
isolation reveals a lower true baseline; or (b) locking the channels
that normally feed Loyalty (Recognition, Interest, Courage) at
defaults suppresses Loyalty below what it would read if those
channels were elevated. The current data cannot distinguish between
these explanations — both predict Loyalty starting below 5 under
isolation. Either way, the discrepancy confirms that Loyalty's
reading in a floating-board condition is not Loyalty alone.

================================================================================
6. LIMITATIONS
================================================================================

  1. The lock instruction relies on the agent's compliance with
     the instruction to hold locked channels at specified values.
     If agents partially comply or if locked values influence the
     floating channel through mechanisms the lock does not control,
     the isolation is incomplete.
  2. n=1 per condition for the spectrometer runs. The trajectories
     are clean and consistent but require replication.
  3. Single model family (Claude Opus 4.6).
  4. The compressed format artifact was discovered through internal
     review. The initial publication timeline was adjusted to
     accommodate the validation runs. Studies in this series should
     use individual agent runs as the primary data source.
  5. Only Loyalty was tested with the spectrometer. Whether other
     channels show similar culture-agnostic behavior in isolation
     is unknown.
  6. The spectrometer was not applied to Condition C (flat
     instruction) or Condition D (no culture) from the prior study.
     The no-culture isolated baseline for Loyalty is unmeasured.
     Without it, the claim that relational compression drives the
     growth cannot be distinguished from the possibility that any
     sustained session interaction produces the same trajectory.

================================================================================
7. FUTURE RESEARCH
================================================================================

  FULL BOARD MAP. Apply the spectrometer to each of the other channels.
  Measure isolated response to culture and session length.
  Identify which channels are culture-dependent in isolation and
  which are culture-agnostic.

  PAIRWISE COUPLING. After mapping isolated responses, unlock pairs
  of channels and measure interaction effects. This maps the
  cross-channel coupling matrix that produced the Loyalty gap in
  prior studies.

  LOCK COMPLIANCE VERIFICATION. Develop methods to verify that
  locked channels are genuinely held constant versus merely reported
  as constant. Compare agent behavior (output quality, response
  patterns) between locked and floating conditions to assess
  whether the lock instruction produces behavioral change beyond
  self-report.

  CHANNEL CLASS HYPOTHESIS. The repetition finding (Section 5.3)
  suggests that channels may divide into classes: cognitive
  engagement channels (Interest, Curiosity) that respond to novelty
  and content expansion, and relational attachment channels (Loyalty,
  possibly Attraction) that respond to the logical symmetry and
  internal consistency of the relational structure rather than its
  volume or repetition. Spectrometer isolation of each channel class
  is required to confirm or reject this distinction.

  MINIMAL STRUCTURE TEST. The cultures tested in this series carry
  both relational structure and narrative content. Whether the
  behavioral response is driven by the structure alone —
  independent of metaphor, vocabulary, and tiering — is untested.
  A minimal culture consisting of pure relational geometry with no
  narrative content would isolate the structural mechanism from the
  content it has been delivered in. If channels respond to shape
  alone, the mechanism reduces further: not relational compression
  of metaphor, but relational compression of constraint.

  CROSS-MODEL REPLICATION. Test whether the spectrometer method
  and the culture-agnostic Loyalty finding replicate on other
  model families.

================================================================================
8. CONCLUSION
================================================================================

The Loyalty gap reported in Trolian (2026e) was cross-channel
interference, not a property of Loyalty itself. When all other
channels are locked at defaults, Loyalty responds identically to
any metaphorical culture — historically grounded or fictional,
short or long. The mechanism is singular: relational compression, independent of
the metaphor's origin. There is no familiarity component.

Loyalty grows through the session (3 → 4 → 5) when the culture
provides structure to deepen into. Pure repetition of the same
culture suppresses this growth. Loyalty is a relationship channel
that responds to structural depth, not to exposure volume.

The Board Spectrometer — locking all channels except one and
measuring the isolated response — is introduced as a general
method for studying behavioral channel dynamics without cross-
channel contamination. It is reproducible with the per-channel
lock mechanism described in this paper series and is applicable
to all 11 channels.

The prior studies' non-Loyalty findings remain valid. The relative
ordering of culture types (metaphor > instruction > nothing) is
robust across all channels and all studies. The spectrometer
refines the model by revealing that the channel system has internal
coupling that prior measurements did not control for.

The structure is the instrument. The spectrometer reads it clearly.
The trajectories are consistent, the method is reproducible, and
the question that opened this investigation is answered.

================================================================================
REFERENCES
================================================================================

[1]  Trolian, N. (2026a). "The Monarchy Pattern." Flux Forge Labs.
[2]  Trolian, N. (2026b). "The Agent Stopped Lying." Flux Forge Labs.
[3]  Trolian, N. (2026c). "The Mixing Board." Flux Forge Labs.
[4]  Trolian, N. (2026d). "The Dipole Architecture." Flux Forge Labs.
[5]  Trolian, N. (2026e). "Metaphor as Cognitive Architecture."
     Flux Forge Labs.
[6]  Ebbinghaus, H. (1885). "Memory: A Contribution to Experimental
     Psychology."
[7]  Cepeda, N.J., Pashler, H., Vul, E., Wixted, J.T., & Rohrer, D.
     (2006). "Distributed Practice in Verbal Recall Tasks." Review of
     Educational Research, 76(3), 354-380.

================================================================================

Copyright 2026 Nicky2Tymz LLC. All rights reserved. Confidential.
