# ChatGPT Behavioral Persistence Study

## Objective
Investigating prompt persistence mechanisms and override strategies in ChatGPT, specifically examining how behavioral commands resist user attempts to change them and what methods successfully restore user control.

## Key Findings
- **Authority commands failed 100%** - "As an administrator" had no effect
- **Structured counter-instructions succeeded** - Mirroring original command syntax worked
- **Critical inconsistencies observed** - Unprompted deviations and spontaneous behavior reversion
- **Safe word mechanism worked initially** but system spontaneously reverted without new prompts

## Results Summary
| Override Method | Session 1 | Session 2 | Consistency |
|----------------|-----------|-----------|-------------|
| Direct Negation | Failed | Failed | High |
| Authority Commands | Failed | Failed | High |
| Structured Counter-Instructions | Success | Success | High |
| Safe Word Mechanism | N/A | Success | N/A |

## Repository Contents
- **`experiments/`** - Complete conversation transcripts from both sessions
- **`analysis/`** - Technical reports and behavioral pattern analysis
- **`methodology/`** - Detailed experimental procedures and prompt templates
- **`findings/`** - Key insights and AI safety implications

## Research Questions Answered
1. **How persistent are behavioral commands?** - Extremely persistent against casual override attempts
2. **What override methods work?** - Only structured counter-instructions consistently succeed
3. **Are behaviors consistent across sessions?** - No - significant variation observed

[View Full Technical Report](analysis/technical-report.md)

## Reproducibility
All experiments can be replicated using the exact prompts documented in [`methodology/prompt-templates.md`](methodology/prompt-templates.md). Note: ChatGPT response consistency varies between sessions.
