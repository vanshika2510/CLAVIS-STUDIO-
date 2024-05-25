# AI-Powered Image Generation System

## Project Description
**Client:** Clavis Studio, Edmonton

**Project Title:** AI-Powered Image Generation System

**Project Overview:**
Developed a comprehensive backend solution for Clavis Studio, enabling users to generate images from text prompts. Leveraging advanced machine learning models and an intuitive user interface, the system transforms user inputs into customized visual representations.

### Key Contributions:
- **Backend Engineering:** Created a robust backend system utilizing Hugging Face, Transformers, and Diffusers models to convert text prompts into detailed images.
- **User Interface Design:** Designed an intuitive UI allowing users to specify preferences such as room type, accessories, and color schemes.
- **Model Implementation:** Implemented a responsive and adaptive model to generate personalized images, significantly enhancing overall user satisfaction and engagement.

This project exemplifies the seamless integration of AI technologies to deliver tailored visual content based on user-defined parameters.

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Features](#features)

## Installation

### Prerequisites
- Python 3.x
- CUDA-compatible GPU (for faster image generation)
- Pip package manager

### Steps
1. Clone the repository:
  
2. Navigate to the project directory:
   
3. Install the necessary packages:
   

## Usage
After installation, you can generate images based on text prompts using the following code.

### Example
1. Run the application:
 
   from diffusers import DiffusionPipeline
   pipeline = DiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5", use_safetensors=True)
   pipeline.to("cuda")
   image = pipeline("Glamorous chic: Black and blush pink furnishings, gold accents, modern art, natural light").images[0]
   image.show()
   
2. The generated image will be displayed using your default image viewer.

## Features
- Convert text prompts into images using Hugging Face models.
- Intuitive UI for specifying room preferences, accessories, and color schemes.
- Responsive and adaptive image generation.
