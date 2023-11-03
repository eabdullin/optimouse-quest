# OptimouseQuest: Synthetic Dataset for Goal-Oriented Question Generation in Optimization Dialogs
## Abstract
Linear programming (LP) problems are ubiquitous in various real-world scenarios. OptimouseQuest aims to facilitate the development of conversational agents that assist users in formulating linear models for these problems. Using prompt engineering, two agents are developed: one simulates a conversational agent and the other, a user. The agents engage in dialogues based on text descriptions of linear problems from NLP4Opt, generating sample conversations that can serve as a baseline for future work.

## Dataset Structure
Human Annotated folder - the dialogues from the DEV subset of NLP4Opt with human evaluation(28 dialogues).   
Dev folder - the dialogues from [DEV](https://github.com/nl4opt/nl4opt-competition/blob/main/generation_data/dev.jsonl) subset of NLP4Opt  
Train folder - the dialogues from [TRAIN](https://github.com/nl4opt/nl4opt-competition/blob/main/generation_data/train.jsonl) subset of NLP4Opt  
```
data/ 
  generated
    human_annotated/* 
    dev/* 
    train/* 
```
## Evaluation
The dataset includes extrinsic evaluation metrics, assessing the quality of dialogue summaries against original problem descriptions. Both human and automatic evaluations have been conducted, including a GPT-4-based approach to mimic human evaluation metrics.
### Human Evaluation
Four evaluators scored how well the summary generated at the end of the dialogue matches the problem statement. For every pair of a problem statement and a generated summary, each evaluator produced the following 4 evaluation metrics.

- **Information recall (IR)** (1-5) -- All the necessary information is in the generated summary.
- **Information precision (IP)** (1-5) -- No irrelevant information is generated.
- **Information repetition (IRep)** (1-5) -- The generated summary does not repeat the same information multiple times.
- **Readability (Read)** (1-5) -- The generated summary is easily readable and fluent.

## Usage
To use this dataset in your project, please follow these steps:

Clone the repository:

```bash
git clone https://github.com/eabdullin/optimouse-quest.git
```
Navigate to the data directory:

## Contributing
If you find any errors or have suggestions, please open an issue or submit a pull request.

## License
This dataset is released under the MIT License.
