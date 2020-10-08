# karabiner_non-modal_vim
A non-modal Vim-like navigation bindings for Karabiner-Elements. It avoids getting confused about which mode you are in, but retains typical vim-like motions.

It is based on harmtemolder's [Vim Mode Plus](https://git.sr.ht/~harmtemolder/karabiner-vim-mode-plus).

It works by assigning the "normal mode" to holding `caps lock`, enabling typical normal-mode motions like `h j k l`. Only simple motions are supported.

## Supported Actions
(incomplete)
While holding down `caps lock`, the following actions are supported:
key | action
--- | ---
`h` | move left
`j`  | move down
`k`  | move up
`l`  | move right
`e`  | move forward to end of word (`option + right arrow`)
`b`  | move back to beginning of word (`option + left arrow`) 
`0`  | move to beginning of line (`cmd + left arrow`) 
`0`  | move to end of line (`cmd + right arrow`) 
`v`  | mark entire line (triple left mouse click?)

All should work with `shift` to select.

## Development
Build json file by running `yml-to-json.py`.
Copy json file into `~/.config/karabiner/assets/complex_modifications/`, then add rules via preferences --> Complex modifications.