# Suckless patches

This repo contains some patches I made for my personal use.

## Slock - XFT message

[This patch](slock-xft-message-20200913.diff) is a modified version of the original [message-patch](http://tools.suckless.org/slock/patches/message/) but using XFT instead. This makes the text nicer to look at and allows for TTF-fonts.

This version doesn't handle tabs like the original one does but it should be fairly simple to add yourself.

## Slock - command

[This patch](slock-command-20200913.diff) is intended to be installed over the [message-patch](http://tools.suckless.org/slock/patches/message/) (official-version, though easily modified to fit the XFT-one) and modifies it to display the output of a command instead of a static text message. The command is re-run at a fixed interval.

You probably shouldn't run anything too CPU-intensive or anything that expects user-input with this patch. It's very likely that the systetm hangs.

## Slock - multiple monitors

[This patch](slock-multi-mon-20201105.diff) is intended to be installed over the [message-patch](http://tools.suckless.org/slock/patches/message/) (official-version, though easily modified to fit the XFT-one) and modifies it such that the message is show in the center of each montior instead of once in the collective center of all monitors. 

