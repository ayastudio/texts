# Vim - save and exit. How to exit Vim. Exit from vi.

> I worked in Vim for two years, because I couldn't figure out a way to exit.
> © Anonimous

![Exit Vim. Hot wo exit vi. Find a way out of Vim. Chicken Run from the terminal.](en.jpg?raw=true)

## Before leaving

Likely, you've already tried lots of different keys, got a million errors, warnings, and many more.

It's time to calm down and take a deep breath. Exhale. Inhale. Exhale.

Now, press the Escape key several times. On the keyboard, it is usually located in the upper left corner, and is labeled "Esc".

Also, switch the layout to English.

If you opened Vim in a remote terminal via ssh, then most likely there is already an English layout enabled.

**So, how do you want to exit?**

- [exit without saving] (#1---exit-without-saving)
- [with saving] (#2---exit-with-saving)

## 1 - Exit without saving

Hold Shift and then successively press Z and then Q

**Alternative option**

Press the colon key,:

Usually, for this you need to hold down Shift and press the semicolon key, ;

Next, in the command line at the bottom of the screen, enter:

q!

## 2 - Exit with saving

Hold Shift, then press Z, then Z again

**Alternative option**

Press the colon key,:

Usually, to do this, you need to hold down Shift and press the semicolon key, ;

Next, in the command line at the bottom of the screen, enter:

wq

## FAQ

> Q: Vim can't save a file and there is an error at the bottom of the screen

Most likely, this is caused by opening a file that your user cannot directly edit.

Then, open a command line by entering a colon, :

Next, while in the command line, enter:

`w! sudo tee%`

And press Enter.

This command tries to save the file using root privileges (administrator, to put it simply). enter password
your user and the file will be saved if your user can request such rights.
It happens that it cannot, which means that your account will not be able to save this file. It's time to ask the admins :(
> Q: Why is Vim so weird?
tl; dr - terminal features, key multiplicity in different modes.
The vi editor, and then its improved version, Vim, began development in the last century. No, that doesn't mean they
bad. But this also does not mean that they are good. It is simply a fact that strongly influenced all decisions in its development.
Vi was created a little later than the advent of the computer mouse, and he himself was written for the ADM-3A terminal, which had a limited
keyboard - without arrow keys, and from the modifier keys there was Shift and a little Ctrl.
> And yes, the terminal in those years was a real, physical thing with a keyboard.
> What is now called a terminal in computers is "terminal emulators".
So, there is only a keyboard and that one is cut. I had to figure out how to use what was available to the maximum.
In vi, and then in Vim, we created a modal interface, i.e. the keys performed different actions in different modes.
There are two main modes: command mode and insert mode. In insert mode, the keyboard is used to enter text, and in
In command mode, the keys move the cursor and modify the text.
Keyboard shortcuts in command mode form their own language, a kind of ordered syntax. It is not immediately visible at the start
vi / Vim is hard to understand right off the bat, but extremely powerful and flexible. If you comprehend it, then it gives all the tools
for quick manipulation of text without taking your hands off the keyboard.
Vim is very easy to customize for yourself, it even has its own programming language - Vim script. But these are unnecessary details.
> Q: Maybe I should start writing in Vim?
If you want to more thoughtfully deal with Vim, or just try it in practice, then I recommend my
(* yes, self-promotion *) config for Vim:
[.Vimrc config file] (https://gist.github.com/novusnota/65dcc593df6d9909ffb59eb83fe69a28)
At the end, there are links to resources that are useful in learning, and it itself is full of explanations about what and how it works.
There is also NeoVim, a rewritten and improved version of Vim, I recommend looking at it too. Good luck!
## That's it guys!
Helpful? Like and subscription to the studio :)
By the way, to keep track of our projects, successes and failures, subscribe to the [email newsletter] (https://gumroad.com/ayast).
No spam and nonsense, we promise.

---

Date: 29.12.2020
| Author: Yakov Gellert (novusnota)
| Translated by: Yakov Gellert (novusnota)

