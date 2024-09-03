# Basic First Aid Q&A Model

This project presents a model that provides clear, step-by-step instructions for basic first aid scenarios. The model is designed to guide users through immediate actions, necessary follow-up care, and advice on when to seek professional help.

## Features

- **Prompt**: The model is optimized with the following prompt:

  > “A model that answers questions about basic first aid with clear, step-by-step instructions for each scenario, including immediate actions, follow-up care, and when to seek professional help.”
-**Dataset**:Created using openai api using the gpt-4 model.
- **Error Handling**: Adjustments have been made to the code to accommodate the updated OpenAI library. An error handling mechanism is implemented to manage API rate limit errors effectively, ensuring continuous operation even when limits are reached.

- **Model Fine-Tuning**: The project also includes fine-tuning of the Llama2 model to enhance its performance in providing accurate and detailed first aid instructions.

## Technologies Used

- **OpenAI API**: Utilized for accessing powerful language models to process the first aid queries.
- **Llama2 Fine-Tuning**: The Llama2 model was fine-tuned to improve its response accuracy for specific first aid scenarios.
- **Google Colab**: The free tier of Google Colab was used for development and fine-tuning, making it accessible without the need for extensive computational resources.
