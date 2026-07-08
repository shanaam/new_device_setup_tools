# Autohotkey
Download autohotkey, place the caps_to_esc.ahk file in [USER]\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup

# vscode_settings
settings and keybinds for vscode
## Settings:
{
    // Personal
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
    // Claude
    "claudeCode.preferredLocation": "panel",
    // Git
    "git.autofetch": true,
    "git.enableSmartCommit": true,
    "git.confirmSync": true,
    // Vim
    "vim.smartRelativeLine": true,
    "vim.useCtrlKeys": false,
    "vim.useSystemClipboard": true,
    // Python
    "editor.defaultFormatter": "charliermarsh.ruff",
    "editor.codeActionsOnSave": {
        "source.organizeImports": "explicit"
    },
    "python.analysis.inlayHints.variableTypes": true,
    "python.analysis.inlayHints.functionReturnTypes": true,
    "pylint.enabled": false,
    // Other
    "dart.flutterSdkPath": "C:\\Users\\smodc\\programs\\flutter",
    "markdown-preview-enhanced.revealjsTheme": "vscode.css",
    "markdown-preview-enhanced.previewTheme": "vscode.css",
    "markdown-preview-enhanced.codeBlockTheme": "vscode.css",
    "markdown-preview-enhanced.enablePreviewZenMode": false,
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

