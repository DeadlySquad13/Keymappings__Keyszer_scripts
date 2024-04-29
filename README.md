# Keymappings Keyszer scripts
Used for low-level system keymappings via `keyszer`.
This program injects into `udev/*` input files to create mappings
to make universal symbol layout possible.

It has quite a lot of possibilities because of it's rich api and python
environment. For example, it can use different keymappings table
depending on current application. But for now [`Keymappings__Engine`](https://github.com/DeadlySquad13/Keymappings__Engine) still seems like
a better candidate because of system-agnostic nature and overall more flexible
api. So for now it's `Keymappings__Engine` domain to create mappings for
interacting with apps, while `ahk`, `karabiner` and `keyszer` better handle
low-level remaps (the reason engine wasn't used for this is because of
intricate problems with `win` key remaps).
