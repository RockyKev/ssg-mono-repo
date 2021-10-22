---
title: TIL about Tmux and persistent terminals
date: 2021-10-09
published: true
tags: ['linux', 'raspberrypi', 'terminal', 'ssh']
series: false
canonical_url: false
description: "Tmux lets you start a terminal session and then open multiple windows inside that session. Tmux sessions are persistent, which means that programs running in Tmux will continue to run even if you get disconnected."
layout: layouts/post.njk
---

I bought a Raspberry Pi 4 a few months ago and struggled to find something to do with it.

I learned recently of a cool way to farm Steam Cards.
But the thing about when you disconnect from a remote computer, the command gets killed.
To explain in a different way:

1. You `ssh` into your raspberry pi
2. You run a command.
3. You watch the command go, and it continues to run.
4. You decide to close the terminal (and kill the connection)
5. The command stops too.

But you want the command to run non-stop. WTH?

To solve that, you'll use something like `Tmux`.

> Tmux is a terminal multiplexer an alternative to GNU Screen . In other words, it means that you can start a Tmux session and then open multiple windows inside that session. Each window occupies the entire screen and can be split into rectangular panes.

> With Tmux you can easily switch between multiple programs in one terminal, detach them and reattach them to a different terminal.

> Tmux sessions are persistent, which means that programs running in Tmux will continue to run even if you get disconnected.

Via the Documentation: https://linuxize.com/post/getting-started-with-tmux/

To install:

`$ sudo apt install tmux`


Once it's up and running:

**To check if there's any windows open:**

`tmux ls`

**To start a new session:**

`tmux new -s session_name_here`

**To detach from a current session:**

`ctrl + b, then d`

**To kill a session:**

`tmux kill-session -t session_name_here`

**To return to a session:**

`tmux a -t session_name_here`

Via the Tmux Cheatsheet: https://tmuxcheatsheet.com/
