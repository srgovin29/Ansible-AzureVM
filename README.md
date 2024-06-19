

sudo apt update
sudo apt install cmake make gcc g++ libssl-dev python3-dev
sudo apt update
sudo apt install python3-pip
pip3 install ansible==8.7.0
pip3 install ansible[azure]

https://github.com/ansible-collections/azure
ansible-galaxy collection install azure.azcollection
pip3 install -r ~/.ansible/collections/ansible_collections/azure/azcollection/requirements.txt
ansible-galaxy collection install azure.azcollection --force

###############################################################################################

# Install virtualenv if not already installed
pip3 install virtualenv

# Create a virtual environment
python3 -m venv ansible-env

# Activate the virtual environment
source ansible-env/bin/activate

# Install Ansible and Azure modules within the virtual environment
pip install ansible==8.7.0
pip install ansible[azure]

# Verify the installation
ansible --version

# To deactivate the virtual environment
deactivate


https://github.com/ansible-collections/azure
ansible-galaxy collection install azure.azcollection
pip3 install -r ~/.ansible/collections/ansible_collections/azure/azcollection/requirements.txt
ansible-galaxy collection install azure.azcollection --force