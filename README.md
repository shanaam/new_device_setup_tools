# vscode_settings
settings and keybinds for vscode


Settings:
{
    "editor.fontSize": 16,
    "editor.bracketPairColorization.enabled": true,
    "editor.guides.bracketPairs": true,
    "editor.guides.bracketPairsHorizontal": true,
    "editor.wordWrap": "on",
    "editor.fontLigatures": true,
    "editor.fontFamily": "Fira Code",
    "workbench.colorTheme": "Night Owl",
    "editor.formatOnSave": true,
    "editor.lineNumbers": "relative",
    "editor.suggestSelection": "first",
    "editor.suggest.snippetsPreventQuickSuggestions": false,
    "git.autofetch": true,
    //vim
    "vim.useCtrlKeys": false,
    "vim.useSystemClipboard": true,
    //c# settings for unity
    "omnisharp.useModernNet": false,
    "editor.tabSize": 2,
    //terminal commands
    "terminal.integrated.profiles.windows": {
        "ctrl init": {
            "source": "PowerShell",
            "args": [
                "-NoExit",
                "-Command",
                "conda activate ctrldev",
            ],
        }
    },
    "terminal.integrated.defaultProfile.windows": "ctrl init",
}

Keybindings:
// Place your key bindings in this file to override the defaults
[
    {
        "key": "ctrl+l",
        "command": "workbench.action.terminal.focusNextPane",
        "when": "terminalFocus && terminalHasBeenCreated || terminalFocus && terminalProcessSupported"
    },
    {
        "key": "alt+down",
        "command": "-workbench.action.terminal.focusNextPane",
        "when": "terminalFocus && terminalHasBeenCreated || terminalFocus && terminalProcessSupported"
    },
    {
        "key": "alt+right",
        "command": "-workbench.action.terminal.focusNextPane",
        "when": "terminalFocus && terminalHasBeenCreated || terminalFocus && terminalProcessSupported"
    },
    {
        "key": "ctrl+k",
        "command": "workbench.action.focusActiveEditorGroup"
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
        "command": "expandLineSelection",
        "when": "textInputFocus"
    },
    {
        "key": "ctrl+l",
        "command": "-expandLineSelection",
        "when": "textInputFocus"
    },
    {
        "key": "shift+j",
        "command": "editor.action.insertCursorBelow",
        "when": "editorTextFocus"
    },
    {
        "key": "ctrl+alt+down",
        "command": "-editor.action.insertCursorBelow",
        "when": "editorTextFocus"
    }
]

