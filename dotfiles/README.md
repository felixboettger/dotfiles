# Felix's Dotfiles

## Install

`git clone --bare https://github.com/felixboettger/dotfiles dotfiles`
`git config --local status.showUntrackedFiles no`

## Setup

If you're not using the included zsh config file, or you are using a different
shell, add an equivalent function to your config:

`dtf () {
  git --git-dir="$HOME/dotfiles" --work-tree="$HOME" "$@"
}`

## Usage

To add a new config file to the repo, use

`dtf add ${.nameofdotfile}`

To commit the change, use

`dtf commit -m "Your commit message"`

To push the change, use 

`dtf push`
