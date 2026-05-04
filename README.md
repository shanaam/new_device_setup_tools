# Autohotkey
Download autohotkey, place the caps_to_esc.ahk file in [USER]\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup

# vscode_settings
settings and keybinds for vscode
## Settings:
{
    //personal
    "editor.fontSize": 16,
    "editor.bracketPairColorization.enabled": true,
    "editor.guides.bracketPairs": true,
    "editor.guides.bracketPairsHorizontal": true,
    "editor.wordWrap": "on",
    "editor.fontLigatures": false,
    "editor.fontFamily": "Fira Code",
    "workbench.colorTheme": "Night Owl",
    "editor.formatOnSave": true,
    "editor.lineNumbers": "relative",
    "editor.suggestSelection": "first",
    "editor.suggest.snippetsPreventQuickSuggestions": false,
    // Git
    "git.autofetch": true,
    "git.enableSmartCommit": true,
    "git.confirmSync": true,
    // Vim
    "vim.smartRelativeLine": true,
    "vim.useCtrlKeys": false,
    "vim.useSystemClipboard": true,
    //c# settings for unity
    "omnisharp.useModernNet": false,
    "editor.tabSize": 2,
    // Python
    "python.terminal.activateEnvironment": true,
    "python.terminal.executeInFileDir": true,
    "terminal.integrated.profiles.windows": {
        "PowerShell": {
            "source": "PowerShell",
            "icon": "terminal-powershell"
        },
        "Command Prompt": {
            "path": [
                "${env:windir}\\Sysnative\\cmd.exe",
                "${env:windir}\\System32\\cmd.exe"
            ],
            "icon": "terminal-cmd"
        },
        "Git Bash": {
            "source": "Git Bash"
        }
    },
    "terminal.integrated.defaultProfile.windows": "PowerShell",
    "terminal.integrated.env.windows": {
        "CONDA_AUTO_ACTIVATE_BASE": "false",
        "CONDA_SHLVL": "0"
    },
    "python.analysis.typeCheckingMode": "basic",
    // Linting and Formatting
    "[python]": {
        "editor.formatOnType": true
    },
    "editor.formatOnSave": true,
    "editor.formatOnSaveMode": "modificationsIfAvailable",
    "editor.codeActionsOnSave": {
        "source.organizeImports": "explicit"
    },
    // Python Formatting
    "pylint.enabled": false,
    // Terminal
    /*
    "terminal.integrated.profiles.windows": {
        "ctrl init": {
            "source": "PowerShell",
            "args": [
                "-NoExit",
                "-Command",
                "conda activate [ENV_NAME]",
            ],
        }
    },
    "terminal.integrated.defaultProfile.windows": [LINE TO RUN AT STARTUP (E.G., XXXX init)],
    //terminal other example
    "terminal.integrated.profiles.windows": {
        "PowerShell": {
            "source": "PowerShell",
            "icon": "terminal-powershell"
        },
        "Command Prompt": {
            "path": [
                "${env:windir}\\Sysnative\\cmd.exe",
                "${env:windir}\\System32\\cmd.exe"
            ],
            "args": [
                "/K",
                "D:\\shanaa\\Programs\\anaconda3\\Scripts\\activate.bat"
            ],
            "icon": "terminal-cmd"
        },
        "Git Bash": {
            "source": "Git Bash"
        }
    },
    "terminal.integrated.defaultProfile.windows": "Command Prompt",
    */
}

Keybindings:
// Place your key bindings in this file to override the defaults
[
  {
    "key": "ctrl+shift+k",
    "command": "-editor.action.deleteLines",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "ctrl+shift+k",
    "command": "workbench.action.terminal.focus",
    "when": "editorTextFocus"
  },
  {
    "key": "ctrl+shift+k",
    "command": "workbench.action.focusActiveEditorGroup",
    "when": "terminalFocus"
  },
  {
    "key": "ctrl+j",
    "command": "-extension.vim_ctrl+j",
    "when": "editorTextFocus && vim.active && vim.use<C-j> && !inDebugRepl"
  },
  {
    "key": "ctrl+shift+j",
    "command": "-workbench.action.search.toggleQueryDetails",
    "when": "inSearchEditor || searchViewletFocus"
  },
  {
    "key": "ctrl+shift+j",
    "command": "workbench.action.togglePanel"
  },
  {
    "key": "ctrl+j",
    "command": "-workbench.action.togglePanel"
  },
  {
    "key": "ctrl+j",
    "command": "workbench.action.terminal.focus"
  },
  {
    "key": "shift+j",
    "command": "cursorDownSelect",
    "when": "editorTextFocus && vim.active && vim.mode == 'Normal'"
  },
  {
    "key": "shift+k",
    "command": "cursorUpSelect",
    "when": "editorTextFocus && vim.active && vim.mode == 'Normal'"
  },
  {
    "key": "alt+shift+j",
    "command": "editor.action.insertCursorBelow",
    "when": "editorTextFocus"
  },
  {
    "key": "alt+shift+k",
    "command": "cursorUndo",
    "when": "editorTextFocus"
  }
]

