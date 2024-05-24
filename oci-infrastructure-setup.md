## OCI Infrastructure Setup

### Step 1: Create a Compartment

A compartment helps you organize and isolate your cloud resources.

1. **Login to OCI Console**:
   - Go to the [OCI Console](https://cloud.oracle.com/) and sign in.

2. **Open the Navigation Menu**:
   - Click the menu icon (three horizontal lines) in the top left corner.

3. **Go to Compartments**:
   - Select "Identity & Security" > "Identity" > "Compartments".

4. **Create a Compartment**:
   - Click "Create Compartment".
   - Enter a name (e.g., "MyCompartment").
   - Optionally, add a description.
   - Choose the parent compartment (usually "root").
   - Click "Create Compartment".

### Step 2: Set Up Networking

Set up a Virtual Cloud Network (VCN) for your instance.

1. **Open Networking**:
   - From the menu, select "Networking" > "Virtual Cloud Networks".

2. **Create a VCN**:
   - Click "Create VCN".
   - Choose "Start VCN Wizard".
   - Enter a name for the VCN (e.g., "MyVCN").
   - Choose your compartment.
   - Enter a CIDR block (e.g., "10.0.0.0/16").
   - Follow the wizard steps to create subnets, an internet gateway, and a route table.

### Step 3: Create an SSH Key

You need an SSH key to securely connect to your instance.

1. **Generate SSH Key on Your Computer**:
   - **Windows**:
     - Use Git Bash or PowerShell.
     - Run: `ssh-keygen -t rsa -b 2048`
   - **macOS/Linux**:
     - Open Terminal.
     - Run: `ssh-keygen -t rsa -b 2048`
   - Follow the prompts. The key files (`id_rsa` for private and `id_rsa.pub` for public) will be created in `~/.ssh/`.

2. **Save Your SSH Key**:
   - Keep the private key file (`id_rsa`) safe.
   - You will need to paste the contents of the public key file (`id_rsa.pub`) later.

### Step 4: Create an Instance

1. **Open Compute**:
   - From the menu, select "Compute" > "Instances".

2. **Create an Instance**:
   - Click "Create Instance".
   - Enter a name (e.g., "MyInstance").
   - Choose your compartment.
   - Select an availability domain.
   - Choose an OS image (e.g., "Oracle Linux").
   - Select an instance shape (e.g., "VM.Standard.E4.Flex").
   - Choose the VCN and subnet created earlier.
   - **Add SSH Key**:
     - Click "Paste SSH Keys".
     - Paste the content of your `id_rsa.pub` file.
   - Click "Create".

### Step 5: Access Your Instance

1. **Get Public IP Address**:
   - In the instance details page, find the public IP address.

2. **Connect via SSH**:
   - **Windows**:
     - Use Git Bash or PowerShell.
     - Run: `ssh -i ~/.ssh/id_rsa opc@<your_instance_ip>`
   - **macOS/Linux**:
     - Open Terminal.
     - Run: `ssh -i ~/.ssh/id_rsa opc@<your_instance_ip>`

Replace `<your_instance_ip>` with the public IP address of your instance.

By following these steps, you'll have a compartment for organization, a networking setup, and a running compute instance in Oracle Cloud Infrastructure. If you encounter any issues, Oracle's support and documentation can provide further assistance.