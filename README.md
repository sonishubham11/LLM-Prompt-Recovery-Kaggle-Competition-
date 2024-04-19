# Kaggle Contest: LLM Prompt Recovery

## Background
In collaboration with Sanath Goutham, I participated in a Kaggle Contest organized by Google on LLM Prompt Recovery. The objective was to identify or recover the original prompt used for rewritten text from the original text.

## Approaches

### First Approach: Chain of Thought Prompting with Mistral 7B Model
We utilized the Mistral 7B Model along with the addition of a mean prompt to the final LLM output. This approach achieved a leaderboard score of 0.65.

#### Notebook
The notebook for this approach can be found in the "Mistral Inference Notebook[0.65]" folder.

### Second Approach: Fine-tuning Gemma 7B-it Model with 4-bit Quantization
For this approach, we fine-tuned the Gemma 7B-it model using a training dataset containing 4000 records. The dataset was composed in a format of chain of thoughts, incorporating thought process, observation, action, and final prompt.

#### Example Training Data
- **Thought:** To understand the desired prompt, I need to carefully analyze and compare the original text with the rewritten text...
- **Observation:** In the rewritten text, there are several changes and additions made to enhance the description...
- **Action:** Based on these observations, I need to recreate the prompt by incorporating the changes and additions...
- **Prompt:** Rewrite this as a hauntingly beautiful description of a forgotten sanctuary.

#### Results
After fine-tuning, the model achieved a leaderboard score of 0.64.

#### Notebook and Files
The notebook files for training and inferencing can be found in the "Gemma-7b-it Training and Inferencing Notebook[0.64]" folder. Additionally, the adapter configuration for the trained model is saved in the "adapter files" folder.

## Leaderboard Performance
We secured the 136th place among other teams in the contest.

