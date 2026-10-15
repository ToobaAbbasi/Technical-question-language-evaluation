# Preliminary Findings

## Research question
Does the language form of a technical question affect response correctness
from Qwen/Qwen3-1.7B?

## Evaluation setup
- Model: Qwen/Qwen3-1.7B
- 10 underlying technical questions
- Four language forms: English, Roman Urdu, Urdu script, and code-switched
- Total: 40 prompts
- Manual correctness scoring on a 0–2 scale

## Preliminary results
- English: mean correctness 1.8/2
- Code-switched: mean correctness 1.8/2
- Roman Urdu: mean correctness 1.4/2
- Urdu script: mean correctness 1.5/2

## Observed failure examples
The model misinterpreted a Roman Urdu question about wireless signal
strength and produced a repetitive, nonsensical response to a Roman Urdu
question about what to do when an AI model does not know an answer.
Some Urdu-script responses were also vague or technically weak.

## Interpretation
This small pilot suggests that response correctness may vary with the
language form of technical questions. It does not establish a general
ranking of language capabilities.

## Limitations
Only 10 underlying questions were tested, and manual scoring involves
judgment. Translation equivalence, topic coverage, and decoding settings
may affect results. The findings need validation on a larger dataset.

## Path forward
Expand the paired question set, verify translations with fluent speakers,
use a consistent scoring rubric, and evaluate more models and technical
topics.
