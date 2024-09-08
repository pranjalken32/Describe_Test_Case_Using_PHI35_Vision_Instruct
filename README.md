# Describe_Test_Case_Using_PHI35_Vision_Instruct
The Image-to-Test-Case Generator is a web application built using Flask and Azure services and Open Source Multimodal LLM PHI3.5_vision_instruct. 

# Flask Application
app.py: The main Flask application file. It contains routes and functions for handling image uploads and interactions with Azure services.
# Azure Integration
Blob Storage: Functions to upload images to Azure Blob Storage and retrieve their URLs
# Prompting Strategy
## Overview
The application uses a structured prompting strategy to guide Azure’s  PHI3.5_vision_instruct in generating detailed image test cases. <br>

The strategy includes:

### System Message: 
The system message sets the context for the AI model, instructing it to act as an assistant for generating test cases based on images.

### User Message: The user message includes:

A request for generating test cases with a specific format (Description, Pre-conditions, Testing Steps, Expected Result).
The image URL and any additional context provided by the user.


# Model Summary
Phi-3.5-vision is a lightweight, state-of-the-art open multimodal model built upon datasets which include - synthetic data and filtered publicly available websites - with a focus on very high-quality, reasoning dense data both on text and vision. The model belongs to the Phi-3 model family, and the multimodal version comes with 128K context length (in tokens) it can support. The model underwent a rigorous enhancement process, incorporating both supervised fine-tuning and direct preference optimization to ensure precise instruction adherence and robust safety measures.

https://huggingface.co/microsoft/Phi-3.5-vision-instruct
