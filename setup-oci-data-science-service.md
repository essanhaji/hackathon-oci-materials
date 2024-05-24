## Setup OCI Data Science Service

This guide assumes you have already created a compartment and set up networking from previous steps. Now, we'll use these resources to set up the Oracle Data Science Service and create a notebook.

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

### Step 2: Create a Notebook Session

1. **Create a Notebook Session**:
   - In your project, click "Create Notebook Session".
   - Enter a name for your notebook session (e.g., "MyNotebookSession").
   - Choose the compartment (e.g., "MyCompartment").

2. **Select the Notebook Shape**:
   - **Without GPU**:
     - Choose a shape like "VM.Standard2.1".
   - **With GPU**:
     - Choose a shape like "BM.GPU2.2".

3. **Configure Networking**:
   - Choose the Virtual Cloud Network (VCN) and subnet you set up previously (e.g., "MyVCN" and "MySubnet").

4. **Create Notebook Session**:
   - Click "Create".

### Step 3: Access Your Notebook

1. **Open the Notebook**:
   - Once the notebook session status changes to "Active", click on the notebook session name.
   - Click "Open JupyterLab". This will open the JupyterLab interface in a new tab.

### Step 4: Using the Notebook

1. **Create a New Notebook**:
   - In JupyterLab, click the "+" button or go to "File" > "New" > "Notebook".
   - Choose the Python kernel.
   - for virtual environment you can clone existing environment.

2. **Run Python Code**:
   - Write and execute Python code in the notebook for your data science tasks.

By following these steps, you extend the use of your previously created compartment and networking setup to create and use Oracle Data Science Service notebook sessions. You can choose to create notebooks with or without GPU resources based on your project requirements. Use the JupyterLab interface to run and manage your data science projects effectively. If you need further assistance, Oracle's support and documentation are available to help.