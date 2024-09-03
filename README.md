# Basic First Aid Q&A Model

This project showcases a model that provides clear, step-by-step instructions for basic first aid scenarios. The model is designed to help users respond to various first aid situations, offering guidance on immediate actions, follow-up care, and advice on when to seek professional help.

## Project Overview

- **Prompt**: The model is based on the following prompt:
  > “A model that answers questions about basic first aid with clear, step-by-step instructions for each scenario, including immediate actions, follow-up care, and when to seek professional help.”

  This prompt was chosen to address a simple and focused problem domain. By avoiding scenarios with significant deviations or complex variations, it was easier to create a manageable dataset for training.

- **Technology Stack**:
  - **OpenAI API**: The model utilizes the OpenAI API to create a dataset with first aid queries.
  - **Llama2 Fine-Tuning**: Llama2 was fine-tuned with the dataset created with gpt-4 to enhance its ability to provide accurate and relevant first aid instructions.
  - **Google Colab**: The free tier of Google Colab was used for development and fine-tuning, offering accessible computational resources.

- **Key Adjustments and Improvements**:
  - **OpenAI Library Update**: The code was updated to be compatible with the latest OpenAI library, ensuring improved functionality and access to new features.
  - **Error Handling**: An error-catching mechanism was implemented to manage OpenAI API rate limit errors effectively. This ensures that the system can pause and retry automatically when rate limits are reached.
  - **Script Update**: The script `gpt_llm_trainer_v2,_with_GPT_3_5_Fine_Tuning.ipynb` was updated to align with these changes, ensuring it works seamlessly with the new OpenAI and fine-tuning requirements.

- **Challenges Encountered**:
  - **PyArrow Installation Issue**: There was an issue with installing the `pyarrow` library. This was resolved by uninstalling and reinstalling the library to ensure proper installation.
  - **Importing `top_k_top_p_filtering`**: This function had to be separately imported from `transformers.generation.utils` due to changes in the library structure.
  - **GPU Limitations**: Towards the end of the script execution, GPU resources were exhausted, which prevented running the final few cells.
  - **Credit Limit for Openai API**: The credit limit impacted the fine-tuning process, influencing the number of examples used to create the dataset..

- **Training Adjustments**:
  - The number of examples was limited to 30 to manage the use of AI credits during dataset creation.
  - The number of epochs was increased to 3 to reduce the loss of the fine-tuned model, ensuring better training performance and accuracy.
