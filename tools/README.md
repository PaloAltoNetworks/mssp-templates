# Using the tools

This directory is used to house utilities that the application can leverage
to manage templates.

### Using the tools

The tools require python3.5 or later to be running in a virtual environment
with required packages installed.

The steps below are for a standard python virtual environment setup.
Python3.6 is used in the example. Python3.5 or python3.7 may also be used.

```bash
cd iron-skillet/tools
python3.6 -m venv env
source env/bin/activate
pip install -r requirements.txt
```


### create_set_spreadsheet.py
Reads the set command .conf files in `internet_gateway/panos/set_commands`
along with the associated metadata.yaml file
to generate a formula-based Excel spreadsheet of loadable set commands.

Output is in the same set_commands directory.





