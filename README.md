# Encode AI Team 7: project-1-chef-gpt

## Project Description

An AI Chef GPT program that helps with the following:
- Provides a detailed recipe if given a name of a dish
- Suggests a dish to make based on listing one or more ingredients
- Provides a critique based on the details you provided on a dish you made

The AI Chef also has several personalities to choose from that affects the tone of the responses.
  1. Emeril Lagasse
  2. Gordon Ramsay
  3. Monica Geller
  4. Jamie Oliver
  5. Nusret Gökçe

### Sample Demo
https://github.com/Encode-AI-Q1-2024-Team7/project-1-chef-gpt/assets/105133922/68c3caa1-9cf0-4b05-bdc4-2e3f1b69dba7

## Instructions

### 1. Clone git repo

### 2. Setting up your keys

1. Log in to [OpenAI](https://platform.openai.com/)
2. Go to [API Keys](https://platform.openai.com/api-keys)
3. Click on `Create new secret key`
4. Name your key
5. Set permissions to `All`
6. Click on `Create secret key`
7. Copy the key and paste it in an `environment variable` named exactly `OPENAI_API_KEY`:

   ```bash
   # Linux/MacOS/Bash on Windows
   export OPENAI_API_KEY="your-api-key-here"
   ```

   ```bash
   # Windows Command Prompt
   set OPENAI_API_KEY=your-api-key-here
   ```

   ```bash
   # Windows PowerShell
   $env:OPENAI_API_KEY="your-api-key-here"
   ```

8. Check if you have the variable set up correctly by running the following command in your terminal:

   ```bash
   # Linux/MacOS/Bash on Windows
   echo $OPENAI_API_KEY
   ```

   ```bash
   # Windows Command Prompt
   echo %OPENAI_API_KEY%
   ```

   ```bash
   # Windows PowerShell
   echo $env:OPENAI_API_KEY
   ```

9. To check if the key is set up correctly without revealing your key in your terminal, you can display it partially by running the following command:

   ```bash
   # Linux/MacOS/Git Bash on Windows
   echo ${OPENAI_API_KEY:0:3}...
   ```

   ```bash
   # Windows Command Prompt
   echo %OPENAI_API_KEY:~0,3%...
   ```

   ```bash
   # Windows PowerShell
   echo ($env:OPENAI_API_KEY).Substring(0,3) + "..."
   ```

10. Check if you have `sk-...` and not just `...`

> For more instructions on how to complete this in different Operational Systems, go to <https://platform.openai.com/docs/quickstart/step-2-set-up-your-api-key>
---
### 3. Setup a Virtual Environment

1. Setup a `Virtual Environment` for the project
   - [Tutorial](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/)
   - Run `python -m venv venv/` (Linux/MacOS) or `py -m venv venv/` (Windows) to create a virtual environment in your project's folder
2. Activate the virtual environment
   - venv [docs](https://docs.python.org/3/library/venv.html)
   - Run `source venv/bin/activate` or `. venv/bin/activate` (Linux/MacOS) or `source venv/scripts/activate` (Windows) to activate the virtual environment
3. Run the following code in your terminal:
    ```text
    pip install openai
    ```
4. Setup keys for recently created `Virtual Environment` (as needed).

---
### 4. Run Program

Run from the root directory of the cloned repo: 
```text
python -m chef_gpt
```
or
```text
python3 -m chef_gpt
```
