# Bachelor Project Questions


## Code
### Question

In `main.cc:7`, there is the line
```c
#include <gdk/gdkkeysyms.h>
```

But I have the compiler error that the `gdk/gdkkeysyms.h` file is not found.

How do you install the `gdk`? Which version of `gtk` are you using?

### Answer (provisional)
I ran the command 
```bash
bear -- make
```
It produced a `compile_commands.json` that the LSP uses to know which
directories to include.
