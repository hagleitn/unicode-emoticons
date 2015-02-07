# unicode-emoticons

[![MELPA](http://melpa.org/packages/unicode-emoticons-badge.svg)](http://melpa.org/#/unicode-emoticons)

Shortcuts to type unicode emoticons in emacs. If you use emacs for chat (jabber, irc etc) and can't remember how to enter:

```
٩(⁎❛ᴗ❛⁎)۶ ┏(-_-)┓┏(-_-)┛┗(-_-﻿ )┓ ¯\_(ツ)_/¯ and (╯°□°）╯︵ ┻━┻
```

This might help. Unicode-emoticons defines a simple minor mode that you can enable for certain major modes to enter these empticons via abbrevs.

## Installation

Install unicode-emoticons from [MELPA](melpa.org) with:

```
M-x package-install RET unicode-emoticons
```

If you like to do things the hard way: Put unicode-emoticons.el into a directory specified by the load-path variable. Alternatively, you can add a directory to the variable by (add-to-list 'load-path "ADDITIONAL_DIRECTORY").

If you put the file in "~/.emacs.d/unicode-emoticons/unicode-emoticons.el" for instance, the following snippet in your .emacs file will load and init the extension.

```lisp
(add-to-list 'load-path "~/.emacs.d/unicode-emoticons/unicode-emoticons.el")
(require 'unicode-emoticons)
```

If you want to enable it for jabber for instance you'd add:

```lisp
(add-hook 'jabber-chat-mode-hook 'unicode-emoticons-mode)
(add-hook 'jabber-chat-mode-hook 'abbrev-mode)
```

## Usage

Next time you open a jabber window (or anytime unicode-emoticons-mode and abbrev-mode are enabled) you can use one of the abbrevs to type emoticons.

For instance. Typing

```
facepalm0
```

will yield

```
(－‸ლ)
```

Seeing a complete list of abbrevs can be accomplished by

```
M-x list-abbrevs RET
```

Enjoy!

```
•_•)
( •_•)>⌐■-■
(⌐■_■)
 ```