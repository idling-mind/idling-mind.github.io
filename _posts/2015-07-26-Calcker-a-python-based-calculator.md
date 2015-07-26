---
layout: post
title: Calcker
excerpt_separator: <!--more-->
---
Calcker, a python based calculator. I was not so happy with the default linux calculator and so I decided to make one for myself.
<!--more-->
Here is a screenshot of Calcker. And a [link to the git](https://github.com/idling-mind/calcker)

![Calcker](/assets/images/calcker.png)

I was bored of using the regular calculator from linux for doing quick calculations. 

These were my problems.

- I use a computer (with a keyboard) and so, the buttons for the numbers didnt have any use to me.
- History!
- Ways to quickly evaluate parts of the expression
- Add brackets as and when I need
- Looks simple and serves the purpose

Basically I wanted a calculator that works for me rather than I work as the calculator wants me to. I had developed a visual basic based calculator long back which worked the way I want. 

It had an expression box where i will enter the expression that I want to evaluate. An answer box, where it will show the result of the calculation live. The answer box will turn red if there is any syntax error in the expression that I have entered. It supported history. Every time you press enter, the expression in the expression box will be copied to the history and the result of the expression substituted in the expression box. If you press spacebar, the expression will be moved to the history without the result being substituted in the expression box.

I read on the web that python interpreter can work as a good calculator. So I basically took my previous calculator idea itself and created the same in python with pygtk. It works quite well for me. I added few more features like select and evaluate. If you select any text, it will be evaluated and its result will be shown in the status bar at the bottom. If you select any text and press 'c' the selected text will be replaced with its result. If you select text and press 'b' the selected text will be surrounded by parentheses. It also supports history, variable substitution, etc.

The script basically works with the help of an eval function in python. But with few modifications.

##Feature list
- Simple interface
- Live calculation (shows syntax errors if any)
- History support
- Quick evaluation of selected text
- Quick way to add parentheses
- Variable substitution
