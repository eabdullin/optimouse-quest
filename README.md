## OptimouseQuest: Synthetic Dataset for Goal-Oriented Question Generation in Optmization Dialogs
Abstract
Linear programming (LP) problems are ubiquitous in various real-world scenarios. OptimouseQuest aims to facilitate the development of conversational agents that assist users in formulating linear models for these problems. Using prompt engineering, two agents are developed: one simulates a conversational agent and the other, a user. The agents engage in dialogues based on text descriptions of linear problems from NLP4Opt, generating sample conversations that can serve as a baseline for future work.

## Dataset Structure
Dev folder - the dialogs from [DEV](https://github.com/nl4opt/nl4opt-competition/blob/main/generation_data/dev.jsonl) subset of NL4OPT
Train folder - the dialogs from [DEV](https://github.com/nl4opt/nl4opt-competition/blob/main/generation_data/train.jsonl) subset of NL4OPT
```
data/ 
  generated 
    dev/* 
    train/* 
```
## Evaluation
The dataset includes extrinsic evaluation metrics, assessing the quality of dialogue summaries against original problem descriptions. Both human and automatic evaluations have been conducted, including a GPT-4-based approach to mimic human evaluation metrics.

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
