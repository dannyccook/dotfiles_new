# Danny's dotfiles

## “What I want in a dotfiles setup“

1. Have no dependencies => Should be executable on a fresh macOS.
2. Be a one-liner => Copy/Paste from my Dotfiles README.md into bash.
3. Idempotent => I want to run and re-run the one-liner without fear of breaking anything.
4. No manual intervention => Apart from initial sudo prompting, “it should not insist on interactive input".
5. Keep secrets secret => Do not put private info into my public dotfiles.

## “How I went about creating my dotfiles setup“

* I created a macOS bootstrapping bash script called setup-mac-os.sh in my Dotfiles repository which printed “Hello World!”.
* macOS comes with bash shell by default so the script will be executable on a fresh macOS.
* I also updated the README.md with a one-liner command to execute that setup-mac-os.sh bash script.
* Keeping the no manual intervention in mind, all requirements were fulfilled.

## Here we go

* On a fresh macOS:
  * Setup my mac with a one-liner 🔥

  ```bash
  curl --silent https://raw.githubusercontent.com/dannyccook/dotfiles/master/setup-mac-os.sh | bash
  curl --silent https://github.com/dannyccook/dotfiles/master/setup-mac-os.sh | bash
  curl --silent https://github.com/dannyccook/dotfiles_new.git
  curl --silent https://github.com/dannyccook/dotfiles_new/blob/master/README.md
  ```

  * Open a Fish shell and execute `compile_vim_plugins` and `install_oh_my_fish` functions.
  * Enter license information of purchased applications.
  * Manually set [un-automatable shortcuts](https://github.com/dannyccook/dotfiles/blob/master/shortcuts/shortcuts.md#un-automatable-shortcuts)
  * Process Dropbox\'s Dotfiles folder.

  * Execute `bootstrap` function freely which in turn executes the bootstrapping script.
