## OCI AI/ML Services

### 1. Generative AI for the enterprise

Unlock the power of generative AI models equipped with advanced language comprehension for building the next generation of enterprise applications. Oracle Cloud Infrastructure (OCI) Generative AI is a fully managed service available via API to seamlessly integrate these versatile language models into a wide range of use cases, including writing assistance, summarization, and chat.

[Explore OCI Generative AI](https://www.oracle.com/uk/artificial-intelligence/generative-ai/generative-ai-service/)

### 2. Generative AI for the enterprise


## Setup OCI AI/ML Services

This guide assumes you have already created a compartment and set up networking from previous steps. Now, we will extend these resources to set up Oracle Cloud Infrastructure (OCI) AI Services.

### Step 1: Create a Data Science Project

1. **Open the Data Science Menu**:
   - From the OCI Console, open the navigation menu (three horizontal lines) in the top left corner.
   - Select "Analytics & AI" > "Data Science".

2. **Create a Project**:
   - Click "Create Project".
   - Enter a name for your project (e.g., "MyDataScienceProject").
   - Select the compartment you created earlier (e.g., "MyCompartment").
   - Optionally, add a description.
   - Click "Create Project".

### Step 2: Set Up AI Services

1. **Open the AI Services Menu**:
   - From the OCI Console, open the navigation menu.
   - Select "AI Services".

2. **Select a Specific AI Service**:
   - Choose the AI service you want to set up. Options include:
     - AI Vision
     - AI Language
     - AI Speech
     - AI Anomaly Detection

### Step 3: Create an AI Service Resource

For each AI service, follow the specific steps to create a resource. Here’s an example for setting up an AI Vision project.

#### Example: Set Up AI Vision

1. **Create AI Vision Project**:
   - Click "Create Project" in the AI Vision section.
   - Enter a name for your project (e.g., "MyAIVisionProject").
   - Select your compartment (e.g., "MyCompartment").
   - Optionally, add a description.
   - Click "Create Project".

2. **Create a Dataset**:
   - Click "Create Dataset".
   - Enter a name for your dataset.
   - Choose the dataset type (e.g., "Image").
   - Select your compartment.
   - Choose the storage location for your dataset (e.g., Object Storage bucket).
   - Click "Create Dataset".

3. **Upload Data to the Dataset**:
   - Upload images or other data relevant to your AI project.

4. **Create a Model**:
   - Once your dataset is ready, create a model by clicking "Create Model".
   - Enter a name for the model.
   - Select your dataset.
   - Configure model settings as needed.
   - Click "Create Model".

### Step 4: Use AI Services in Your Applications

1. **Access API Endpoints**:
   - Each AI service provides API endpoints that you can use to integrate AI capabilities into your applications.
   - Refer to the OCI documentation for API details specific to each service.

2. **Example Integration**:
   - For AI Vision, you might use the API to analyze images in your applications.
   - For AI Language, you might use the API to process text for sentiment analysis or entity recognition.

By following these steps, you can extend the use of your previously created compartment and networking setup to set up and use OCI AI Services. You have the flexibility to choose from various AI services such as AI Vision, AI Language, AI Speech, and AI Anomaly Detection based on your project needs. Use the provided API endpoints to integrate the power of these AI services into your applications. If you encounter any issues, Oracle's support and documentation are available to help.

