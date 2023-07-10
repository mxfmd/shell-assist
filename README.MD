# Shell Assist

A shell and python script that integartes with OpenAI chat model to suggest a shell command for a user task.

Example:

```shell
➜  shell-assist ./shell_assist.sh "List ports which are in use on Mac"
lsof -i -P | grep LISTEN
```

> **Warning**
> Be very careful with what tools suggested and execute the generated code with care!

## Get Started

1. Add OPENAI_API_KEY from OpenAI to environment variables following the guide: https://help.openai.com/en/articles/4936850-where-do-i-find-my-secret-api-key

E.g. setting up the environment variable for the MacOS (replace 'yourkey' with your own API key):

```shell
echo "export OPENAI_API_KEY='yourkey'" >> ~/.zshrc
source ~/.zshrc
```

2. Install Python's OpenAI module from requirements.txt:

```shell
pip install -r requirements.txt
```

or directly:

```shell
pip install openai
```

3. [Optional] Add to script to PATH:

```shell
export PATH="$PATH:{your path to script}"
```

## Acknowledgments

https://askcommand.com

I've got an inspiration from Ask Command. Whether it is a great app and I suggest rather to use it instead of my script, I took their reluctance of having CLI as an opportunate for this side project - to play with Python and OpenAI api.
