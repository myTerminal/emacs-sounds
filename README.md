# emacs-sounds

[![Marmalade](https://img.shields.io/badge/marmalade-available-8A2A8B.svg)](https://marmalade-repo.org/packages/emacs-sounds)  
[![License](https://img.shields.io/badge/LICENSE-GPL%20v3.0-blue.svg)](https://www.gnu.org/licenses/gpl.html)

Sound effects for Emacs.

You can use emacs-sounds to get visible feedback from Emacs for various events, including the bell.

## Installation

### Manual

Save the file *emacs-sounds.el* to disk and add the directory containing it to `load-path` using a command in your *.emacs* file like:

    (add-to-list 'load-path "~/.emacs.d/")

The above line assumes that you've placed the file into the Emacs directory '.emacs.d'.

Start the package with:

    (require 'emacs-sounds)

### Marmalade

If you have Marmalade added as a repository to your Emacs, you can just install *emacs-sounds* with

    M-x package-install emacs-sounds RET

## Usage

Enable emacs-sounds-mode globally.

    (emacs-sounds-mode)

You need to configure your own sounds for the package to be able to work.

Set `emacs-sounds-bell-sound`, `emacs-sounds-window-change-sound` and `emacs-sounds-find-file-sound` with paths of sound files to be played at the respective events.

    (setq emacs-sounds-bell-sound
        "/home/ismail/sounds/sound1.wav")

You just need to remember that the sound files must be '.wav' audio files.

## Dependencies

* [sound-wav](https://github.com/syohex/emacs-sound-wav)
