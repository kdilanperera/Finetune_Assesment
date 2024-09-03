# Basic First Aid Q&A Model

This project presents a model designed to answer questions about basic first aid by providing clear, step-by-step instructions for each scenario. The model covers immediate actions, follow-up care, and advice on when to seek professional help.

## Project Overview

- **Prompt**: The model is based on the following prompt:
  > “A model that answers questions about basic first aid with clear, step-by-step instructions for each scenario, including immediate actions, follow-up care, and when to seek professional help.”

  This specific prompt was chosen to keep the problem domain simple and focused, minimizing deviations and variations. This simplicity made it easier to create a structured dataset for training the model.

- **Technologies Used**:
  - **OpenAI API**: Used for accessing language models and processing first aid queries.
  - **Llama2 Fine-Tuning**: The model was fine-tuned using Llama2 to enhance its accuracy and specificity in the domain of first aid.
  - **Google Colab**: The development and fine-tuning process utilized Google Colab's free tier for easy access to computational resources.

- **Code Adjustments**:
  - The code was updated to work with the new OpenAI library, ensuring compatibility and leveraging the latest features.
  - An error-handling mechanism was implemented to manage OpenAI API rate limit errors, enabling the system to pause and retry automatically when limits are reached.

- **Challenges**:
  - **PyArrow Library Issue**: During the setup, there was an installation problem with the `pyarrow` library. This was resolved by uninstalling and reinstalling the library to ensure it was installed correctly.
  - **Importing `top_k_top_p_filtering`**: This function had to be separately imported from `transformers.generation.utils` due to changes in the library structure.
  - **GPU Limitations**: Towards the end of the script, GPU resources ran out, preventing the execution of the final few cells.

- **Script Update**: The script named `gpt_llm_trainer_v2,_with_GPT_3_5_Fine_Tuning.ipynb` was updated to align with these requirements and ensure proper functionality with the latest OpenAI and fine-tuning methodologies.
