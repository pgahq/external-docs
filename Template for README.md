# [human-readable repo name here]

[basic description of the repo, the value it provides, and how it works]

## Install
If you don't already have poetry:

```
brew install poetry
poetry self update
```

Clone the repo. CD into it.

Install:

```
poetry install
```

[additional setup instructions here e.g.
Rename `.env.example` file to `.env` and configure keys, IDs, etc.
]

## Run in the virtual environment

`poetry run python main.py`

## Debug / run from VS Code or Cursor

Select your Python interpreter: Press cmd+shift+p to open the Command Palette, start typing "Python: Select Interpreter", and select it when it comes up. This will show you a list of available interpreters that VS Code can find automatically, including virtual environments. Select the virtual environment.

Set up debugging: Go to the Run view in VS Code (cmd+shift+d), and click "create a launch.json file". In the dropdown that appears, select "Python File". This will create a launch.json file in a .vscode folder in your project, and open it in the editor. Use this and `change the args to your liking`:

```
{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Python: [human-readable repo name here]",
      "type": "python",
      "request": "launch",
      "program": "${workspaceFolder}/main.py",
      "args": [],
      "console": "integratedTerminal",
      "justMyCode": true
    }
  ]
}
```

## Configuration
[relevant info here]

## TODO
* [List of items...]