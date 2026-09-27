# Assignments and assessment

## Structured assessment reference

The YAML below is a planning index. The full assessment text and rubrics follow.
`null` means not supplied, not that a requirement does not apply. Rubric weights
are percentages of their component, not of the whole course.

```yaml
course: INF2573
total_grade_percent: 100
source: "User-supplied Section 5: Assessment and Grading"
due_date_authority: "Section 6 course schedule (not supplied)"
course_learning_outcome_definitions: null # Section 2 not supplied
academic_integrity_policy: null # Section 8 not supplied
assessment_principle: "Reward documented learning, disciplined process, and rigour over final-object polish."
components:
  - id: group_project
    weight_percent: 40
    outcomes: [CLO1, CLO2, CLO3, CLO4, CLO5, CLO6]
    team_size: {min: 3, max: 5}
    duration_weeks: 12
    due_date: null
    requirements:
      - "Develop an AI-enabled service from a Week 1 sketch to a defensible working demo."
      - "Frame a testable hypothesis and strategic bet."
      - "Document experiments, iteration, validation, risk, governance, and design rationale."
      - "Define human/AI boundaries and a measurable north-star metric."
      - "Show personal contribution to experiments and build, with evidence behind team claims."
    rubric_percent:
      framing: 15
      scope: 10
      build_and_iteration: 20
      validation: 20
      north_star_metric: 10
      ethics_and_governance: 15
      design_rationale: 10
    failure_conditions:
      - "No personal contribution to team experiments and build."
      - "Team cannot produce evidence behind its claims."
  - id: participation
    weight_percent: 20
    outcomes: [CLO1, CLO2, CLO3, CLO4, CLO5, CLO6]
    cadence: weekly_studio
    requirements:
      - "Arrive prepared, engage in discussion, give actionable critique, and visibly integrate feedback."
      - "Keep evidence of spikes, pretotypes, evaluations, failures, and lessons."
    rubric_percent:
      presence_and_preparedness: 15
      discussion_engagement: 15
      critique_given: 20
      critique_taken: 15
      experiment_trail: 20
      learning_from_failure: 15
    failure_conditions:
      - "Sustained absence from critique."
      - "Repeatedly unprepared with nothing to show or ask."
  - id: logbook
    weight_percent: 20
    outcomes: [CLO1, CLO2, CLO4, CLO5]
    entry_count_required: 8
    format: individual_physical_or_digital
    working_file: Logbook.md
    due_dates: null
    requirements:
      - "Connect weekly readings to real team decisions."
      - "Reflect specifically and honestly on personal contribution, uncertainty, and change."
      - "Reason about socio-technical and macro-economic implications."
      - "Disclose AI use in every entry."
    rubric_percent:
      reading_to_project_connection: 30
      individual_contribution_reflection: 20
      macro_systemic_reflection: 20
      reflective_honesty: 20
      consistency_and_completeness: 10
    ai_policy:
      research_and_thinking_aid: allowed
      disclosure: required_per_entry
      gate: pass_fail_unweighted
      undisclosed_use_consequence: "Fails the gate for that entry."
    failure_conditions:
      - "Missing logbook."
      - "Perfunctory entries or summary without reflection."
  - id: mini_essays
    weight_percent: 20
    outcomes: [CLO1, CLO2, CLO4, CLO5]
    essay_count: 2
    scoring: "Mark each essay with the rubric; average the two."
    deliverables:
      - {id: mini_essay_1, due_week: 5, due_date: null}
      - {id: mini_essay_2, due_week: 10, due_date: null}
    minimum_readings_per_essay: 2
    word_count: null
    requirements:
      - "Take and defend an argumentative thesis across two or more readings."
      - "Demonstrate independent critical judgment about AI and human agency."
      - "Write the prose yourself."
    rubric_percent:
      thesis_and_stand: 25
      critical_engagement: 30
      independent_judgment: 20
      craft_and_articulation: 25
    ai_policy:
      research_and_discovery: allowed_with_disclosure
      ai_generated_writing: prohibited
      gate: pass_fail_unweighted
      gate_requirements:
        - "Engages at least two readings."
        - "No AI-generated writing."
        - "AI research/discovery use disclosed."
      failure_consequence: "Caps or voids the essay per Section 8 Academic Integrity policy."
```

## Full assessment text and rubrics

Transcribed from the supplied text; headings and tables are formatted for Markdown.

### 5. Assessment and Grading
This course is graded out of 100%. Assessment rewards disciplined process over a polished final object: a team can demo something slick and learn nothing, or stumble in the demo and learn enormously. We credit the learning and the rigour.

The four components below are weighted to a grade out of 100%; for each, what good looks like describes the standard you're working toward. Slippage in any single week is fine; a sustained pattern is not. In each rubric, the Proficient level is solid, passing work and Exemplary is what strong work looks like. Outcome codes (CLO1–CLO6) refer to the six Course Learning Outcomes in Section 2.

For all due dates for deliverables, please refer to the schedule outlined below under Number 6.

| Component | Weight | Outcomes | Relation to Course Learning Outcomes |
| --- | --- | --- | --- |
| Group Project | 40% | CLO1–6 | The full design arc — framing, agency boundaries, validation, governance, rationale, and the working demo |
| Participation | 20% | CLO1–6 | Weekly critique and the documented experiment trail rehearse the whole project in progress |
| Logbook (8 entries) | 20% | CLO1, CLO2, CLO4, CLO5 | Connects each week's reading to a real team decision, its risks, and your own contribution |
| Mini essays (2) | 20% | CLO1, CLO2, CLO4, CLO5 | Written, independent critical judgment putting two or more readings in tension |
### A. Group Project (40%) — team of 3–5
What it is. One project, built across twelve weeks. Your team takes an AI-enabled service concept from a rough Week 1 vibe-coded sketch to a defensible demo, treated throughout as a hypothesis and a strategic bet, not a technology or a solution looking for a problem. You are assessed on the argument for the design: framing, scope, iteration, validation, a north-star metric, governance, and rationale, not on the polish of the final object. Big pivots are fine, as long as they carry a clear line of learning from earlier iterations.

What good looks like. A working demo backed by documented experiments, an honest risk analysis, and a clear design rationale. A team whose concept "fails" but documented why, and what they would do next, passes comfortably. You do not pass this component if there is no personal contribution to your team's experiments and build, or if the team cannot produce evidence behind its claims.

#### Rubric

| Criterion (weight) | Exemplary | Proficient | Developing | Inadequate |
| --- | --- | --- | --- | --- |
| Framing (15%): hypothesis + strategic bet | Sharp, non-obvious hypothesis framed as a real bet about desirability, feasibility, and agency; clearly not a solution hunting for a problem | Clear hypothesis and a defensible bet; framing mostly problem-led | Framing present but tech-led or vague; the "bet" is implicit | Solution in search of a problem; no testable hypothesis |
| Scope (10%): human/AI boundaries + right-sizing | Human vs. AI boundaries drawn deliberately and defended; scope ambitious yet achievable | Boundaries defined; scope reasonable | Boundaries fuzzy; scope too big or too small | No boundary reasoning; scope unworkable |
| Build & iteration (20%): each iteration built on prior learning | Clear through-line: every iteration, pivots included, visibly carries learning from the last | Iterations build on each other; line of learning mostly legible | Some iteration but weakly connected; changes look arbitrary | One build, or pivots with no line of learning |
| Validation (20%): hypothesis tested | Hypothesis genuinely tested through experiments, evals, and research; evidence read honestly, including disconfirming results | Tested with credible evidence; reading of it mostly honest | Thin or cherry-picked evidence; testing gestured at | Assertion without evidence |
| North-star metric (10%): a real measure of success | A defensible north-star metric with a working way to measure it, tied to the hypothesis | Metric named and measurable; link to success clear | Metric vague or unmeasured; a vanity metric | No metric; no notion of success |
| Ethics & governance (15%): risk, agency, systemic effects | Serious engagement with risk, human agency, and socio-technical/macro-economic effects; governance (transparency, escalation) designed in | Solid risk and agency analysis; governance addressed | Ethics acknowledged but shallow or bolted on | Absent or box-ticking |
| Design rationale (10%): the argument for the design | Every major choice justified against evidence and the human-agency stakes | Choices mostly justified | Rationale asserted, not argued | Choices unexplained |
Build & iteration plus Validation together carry 40% of the project, more than framing and polish combined. That weighting keeps honest, learning-rich work scoring above a slick demo that learned nothing.

### B. Participation (20%)
What it is. The graded record of how you show up to a working studio. This is not attendance. It credits your visible trail of experimentation (spikes, pretotypes, evals, including ones that failed and what they taught) and your conduct in critique in both directions: the quality of the critique you give, and how you take and integrate critique on your own work. You are assessed on what you do and leave evidence of in the room, not on a general impression.

Why it matters. Critique is not a delivery mechanism for grades; it is a professional skill this course explicitly teaches (Learning Outcome 5). Design judgment gets sharper by being articulated and contested in a room. A team that skips critique loses the fastest feedback loop available to it, and the individual who never gives critique never develops the muscle.

What good looks like. Regular, prepared participation with a documented experiment trail, including failures. You do not pass this component if there is a sustained pattern of absence from critique, or you are repeatedly unprepared with nothing to show or ask.

#### Rubric

| Criterion (weight) | Exemplary | Proficient | Developing | Inadequate |
| --- | --- | --- | --- | --- |
| Presence & preparedness (15%) | Consistently present, readings done, ready to build | Usually prepared | Often unprepared or absent | Rarely present or ready |
| Discussion engagement (15%) | Advances discussion with substance | Contributes regularly | Occasional or surface-level | Disengaged |
| Critique given (20%) | Specific, generous, actionable critique of others' work | Useful critique | Vague or rare | None |
| Critique taken (15%) | Integrates feedback visibly; non-defensive | Receptive to feedback | Resistant | Rejects feedback |
| Experiment trail (20%) | Rich, documented trail of spikes, pretotypes, and evals | Regular logged experiments | Sparse | No trail |
| Learning from failure (15%) | Surfaces failures and what they taught | Acknowledges failures honestly | Hides or ignores them | Denies failure |
The two heaviest criteria, critique given and experiment trail, are the ones backed by reviewable artifacts, so most of this grade rests on evidence, not impression.

### C. Logbook (20%) — 8 entries
What it is. A running individual record (physical or digital), kept alongside the team project. It does connective work the essays and the project can't: it ties each week's reading to a decision your team actually made, tracks your own contribution to the team honestly, and reasons about the macro/systemic implications of what you're building. It is the one place you disclose AI use: AI is allowed here as a research and thinking aid, and what's assessed is the honesty and quality of the connection you draw, not the prose.

What good looks like. 8 substantive entries that consistently and thoughtfully connect ideas to your team's decisions, honest about doubt and change. You do not pass this component if the logbook is missing, entries are perfunctory, or they summarize without reflecting.

#### Rubric

| Criterion (weight) | Exemplary | Proficient | Developing | Inadequate |
| --- | --- | --- | --- | --- |
| Reading → project connection (30%) | Each reading tied to a real team decision with insight | Clear connections drawn | Loose or generic links | Reading and project stay separate |
| Individual contribution reflection (20%) | Honest, specific account of your own role and growth | Reflects on contribution | Vague ("I helped") | Absent |
| Macro/systemic reflection (20%) | Reasons about socio-technical and macro-economic implications of the project | Considers wider implications | Mentioned superficially | None |
| Reflective honesty (20%) | Candid about uncertainty, mistakes, disagreement | Mostly candid | Performative or tidy | Hollow |
| Consistency & completeness (10%) | 8 substantive, on-time entries | 7–8 solid entries | Missing or thin entries | Few entries |
AI disclosure gate (pass/fail, not weighted). AI use for research or thinking is allowed and must be disclosed per entry. Undisclosed use fails the gate for that entry.

### D. Mini Essays (20%) — 2 essays
What it is. Two short argumentative essays on the readings, the first due in Week 5 and the second in Week 10. Each takes a thesis and a stand (agreeing with, criticizing, or putting into tension two or more readings) and defends it. This is where you exercise critical judgment about AI and human agency as a writer, not a builder.

No AI for the writing. AI is fine for research and discovery there, disclosed, but the prose must be your own. What's assessed is your own judgment and argument, not information coverage.

What good looks like. A clear argued position in your own words, engaging two or more readings, with no AI-generated writing.

#### Rubric (mark each essay on this; average the two)

| Criterion (weight) | Exemplary | Proficient | Developing | Inadequate |
| --- | --- | --- | --- | --- |
| Thesis & stand (25%) | A clear, arguable thesis takes a real position across 2+ readings | Clear thesis; position present | Thesis vague or mostly summary | No thesis; book-report |
| Critical engagement (30%) | Puts readings in genuine tension or dialogue; goes beyond what any one says | Engages readings critically | Describes readings; little critique | Misreads or ignores the texts |
| Independent judgment (20%) | Your own judgment is unmistakable and earned | Own view present and supported | View thinly asserted | No discernible own view |
| Craft & articulation (25%) | Tightly argued, well structured, precise voice | Clear and well organized | Loose structure; unclear passages | Hard to follow |
Integrity gate (pass/fail, not weighted). Engages 2+ readings; no AI-generated writing; AI research or discovery use disclosed. Failing the gate caps or voids the essay per the Academic Integrity policy in Section 8.
