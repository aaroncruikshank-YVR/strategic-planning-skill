# Strategic Planning Skill for Claude

A comprehensive strategic planning system for Claude (Cowork / Claude Code), synthesizing frameworks from 18 foundational strategy books into an actionable quarterly planning and implementation workflow.

Built for small teams (2-10 people) who want rigorous strategic thinking without hiring a strategy consultant.

## What It Does

This skill turns Claude into a strategic planning advisor that guides you through two modes:

**Quarterly Planning Sessions** -- a structured deep-work session every 90 days:
1. **Strategic Diagnosis** -- Understand what's actually happening before making decisions (Rumelt)
2. **Strategic Direction** -- Make clear choices about where to compete and how to win (Lafley/Martin)
3. **90-Day Execution Plan** -- Set Rocks, scorecards, and meeting rhythms (Wickman/EOS)
4. **Validation** -- Stress-test the plan for coherence and blind spots (Porter, Christensen)

**Ongoing Implementation Support** -- between quarterly sessions:
- Mid-quarter Rock check-ins
- Ad-hoc strategic decisions (market entry, pricing, hiring, partnerships)
- Scaling diagnostics
- Competitive response analysis

## Frameworks Included

The skill draws on these books and their core frameworks:

| Book | Author(s) | Key Frameworks |
|------|-----------|----------------|
| Good Strategy Bad Strategy | Richard Rumelt | The Kernel (Diagnosis/Guiding Policy/Coherent Actions), Sources of Power |
| Playing to Win | A.G. Lafley & Roger Martin | Strategic Choice Cascade, Reverse Engineering |
| Competitive Strategy | Michael Porter | Five Forces, Three Generic Strategies, Competitor Analysis |
| Traction | Gino Wickman | EOS, V/TO, Rocks, Level 10 Meetings, IDS, Scorecard |
| Value Proposition Design / Business Model Generation | Alexander Osterwalder | Value Proposition Canvas, Business Model Canvas |
| Blue Ocean Strategy | W. Chan Kim & Renee Mauborgne | Strategy Canvas, Four Actions (ERRC), Six Paths, Tipping Point Leadership |
| Crossing the Chasm | Geoffrey Moore | Technology Adoption Lifecycle, Beachhead Strategy, Bowling Pin Model |
| The Innovator's Dilemma / Solution / DNA | Clayton Christensen | Disruption Theory, RPV Framework, Jobs-to-Be-Done |
| The Lean Startup | Eric Ries | Build-Measure-Learn, MVP, Innovation Accounting, Pivot Types |
| Built to Last | Jim Collins & Jerry Porras | Core Ideology, BHAGs, Preserve the Core / Stimulate Progress |
| Scale | Jeff Hoffman & David Finkel | Level Three Road Map, Three-Legged Stool, Self-Employment Trap |
| The Art of Strategy | Avinash Dixit & Barry Nalebuff | Game Theory for Business, Backward Induction, Commitment |
| Practice Game Theory | Albert Rutherford | Nash Equilibrium, Credibility Analysis, Subgame Perfect Equilibrium |
| Strategic Management | Hitt, Ireland & Hoskisson | VRIO Framework, Competitive Dynamics, I/O vs. Resource-Based Models |
| Your Next Five Moves | Patrick Bet-David | Five Moves Framework, Personal Identity Audit |
| Your Strategy Needs a Strategy | Reeves, Haanaes & Sinha | Strategy Palette (Classical/Adaptive/Visionary/Shaping/Renewal) |
| Las Decisiones Estrategicas | Marcel Planellas | Strategic Decision Circle, 30 Models Catalog |
| HBR's 10 Must Reads on Strategy | Various | Balanced Scorecard, RAPID Decisions, Strategy Execution |

## Installation

### Option 1: Install the .skill file (recommended)

Download `strategic-planning.skill` from this repo and install it in Claude Cowork or Claude Code.

### Option 2: Manual installation

Copy the `skill/` directory into your Claude skills folder:

```
~/.claude/skills/strategic-planning/
  SKILL.md
  references/
    analysis-frameworks.md
    strategy-formulation.md
    execution-implementation.md
    game-theory-competitive.md
```

## Usage

Once installed, trigger the skill with prompts like:

```
"Let's run a quarterly strategic planning session"
"I'm evaluating whether to enter a new market segment"
"What should we focus on this quarter?"
"Help me think through our competitive positioning"
"I need to make a pricing decision"
"Are we stuck in the middle strategically?"
"Walk me through a Five Forces analysis of our industry"
```

The skill automatically selects the right framework for the question and reads only the relevant reference file, keeping context efficient.

## Repo Structure

```
strategic-planning-skill/
  README.md
  LICENSE
  .gitignore
  strategic-planning.skill      # Packaged installer
  skill/                        # The skill source files
    SKILL.md                    # Main skill (router + workflow)
    references/
      analysis-frameworks.md    # Diagnosis & analysis tools
      strategy-formulation.md   # Strategy creation frameworks
      execution-implementation.md  # Execution & scaling tools
      game-theory-competitive.md   # Competitive dynamics & game theory
  templates/                    # Blank planning templates
    vision-traction-organizer.md
    quarterly-rocks.md
    weekly-scorecard.md
    level-10-meeting-agenda.md
    strategic-diagnosis.md
    choice-cascade.md
    competitor-analysis.md
    issues-list.md
  examples/                     # Example outputs
    quarterly-planning-session.md
    mid-quarter-check-in.md
```

## Templates

The `templates/` directory contains blank, fillable versions of the key planning documents referenced by the skill. Use these as starting points for your own planning sessions, or let Claude fill them in during a session.

## Examples

The `examples/` directory shows what a completed quarterly planning session and a mid-quarter check-in look like when using the skill. These use a fictional consulting firm to illustrate the workflow.

## Customization

The skill is built for a small professional services / consulting firm, but the frameworks are universal. To adapt it:

1. Edit `skill/SKILL.md` to change the business context in the system prompt section
2. The reference files are framework-agnostic and rarely need changes
3. Add industry-specific templates to `templates/`

## License

MIT License. See [LICENSE](LICENSE).

## Contributing

Issues and PRs welcome. If you've found a framework that should be included or have improvements to the templates, open a PR.
