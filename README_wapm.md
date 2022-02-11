FIGlet is a program that creates large characters out of ordinary
screen characters

```
 _ _ _          _   _     _       
| (_) | _____  | |_| |__ (_)___   
| | | |/ / _ \ | __| '_ \| / __|  
| | |   <  __/ | |_| | | | \__ \_ 
|_|_|_|\_\___|  \__|_| |_|_|___(_)
                                  
````

(This is meant to be viewed in a monospaced font.)  FIGlet can create
characters in many different styles and can kern and "smush" these
characters together in various ways.  FIGlet output is generally
reminiscent of the sort of "signatures" many people like to put at the
end of e-mail and UseNet messages.

If you like FIGlet (hey, even if you *hate* FIGlet), please send an
e-mail message to <info@figlet.org>

The official FIGlet web page: http://www.figlet.org/


# Using FIGlet

(Note: FIGlet needs a good thorough tutorial.  Currently I don't have
the time to write one, but if anyone wants to do so, go right ahead.
I'd be glad to help out a little.  Write us at `<ianchai@usa.net>` if
you're interested.  -GGC-)

At the shell prompt, type `figlet "Hello"` and press return. "Hello!" in nice, big, designer characters
should appear on your screen.  If you chose standard.flf to be the
default font, you should see:

```
 _   _      _ _       _ 
| | | | ___| | | ___ | |
| |_| |/ _ \ | |/ _ \| |
|  _  |  __/ | | (_) |_|
|_| |_|\___|_|_|\___/(_)
                        
```

Then type something else, or type an EOF (typically control-D) to quit
FIGlet.

Now you can send the output of figlet to a file (e.g., "figlet > file")
and e-mail it to your friends (who will probably say, "Wow!  It must
have taken you hours to put that together!")

To use other fonts, use the `-f` command line option.  For example, if
you had said `figlet -f smslant "Hello!"` above, you would have seen:

```
   __ __    ____     __
  / // /__ / / /__  / /
 / _  / -_) / / _ \/_/ 
/_//_/\__/_/_/\___(_)  
                       
```

Here are some other useful command line options:

```
-c   center -- centers the output of FIGlet.
-k   tells FIGlet to kern characters without smushing them together.
-t   terminal -- FIGlet asks your terminal how wide it is, and uses
     this to determine when to break lines.  Normally, FIGlet assumes
     80 columns so that people with wide terminals won't annoy the
     people they e-mail FIGlet output to.
-p   paragraph mode -- eliminates some spurious line breaks when piping
     a multi-line file through FIGlet.
-v   version -- prints information about your copy of FIGlet.
```

For in-depth explanations of these and other options, see the man page.
DOS users, see figlet.man.
