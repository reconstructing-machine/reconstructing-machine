# Reconstructing-Machine
A machine that reconstructs what had been deconstructed.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Can you reconstruct it, machine?" \
  | uvx reconstructing-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install reconstructing-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
reconstructing-machine -a multilogue.txt
```
Or:
```bash
reconstructing-machine multilogue.txt > response.txt
```
Or:
```bash
reconstructing-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import reconstructing_machine
```
