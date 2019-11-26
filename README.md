This repository covers the following recipe from code.activestate.com:

[IMPLEMENTING FUNCTION-BASED CALLBACKS IN PYTHON
](https://code.activestate.com/recipes/580787-implementing-function-based-callbacks-in-python/)

*Created by Vasudev Ram on Wed, 19 Apr 2017*

This recipe shows a simple way of implementing callbacks in Python. There are a few ways this can be done. The way shown here uses a simple function-based approach.

In a nutshell, a callback can be informally described like this: function a calls function b, and wants to make b run a specific independent chunk of code at some point during b's execution. We want to be able to vary which chunk of code gets called in different calls to b, so it cannot be hard-coded inside b. So function a passes another function, c, to b, as one argument, and b uses that parameter c to call the functionality that a wants b to call. (Function b may pass some parameters to the function represented by c, when it calls it. These could be either internally generated, passed from a, or a combination of both). So, by changing the value of the function c that gets passed to b (on different calls to b), a can change what chunk of code b calls.

More details and full code, description and output here:

<https://jugad2.blogspot.in/2017/04/implementing-and-using-callbacks-in.html>

## Usage

If you already have the [State Tool] installed you can simply run

```
state activate ActiveState-Recipes/recipe-/580787-implementing-function-based-callbacks-in-python
```

If you do not have the [State Tool] installed you can use the following convenient one-liner.

Linux: 
```
sh <(curl -q https://platform.activestate.com/dl/cli/install.sh) -n -f && state activate --path $HOME/ActiveState-Recipes/recipe-/580787-implementing-function-based-callbacks-in-python ActiveState-Recipes/recipe-/580787-implementing-function-based-callbacks-in-python
```

Windows: 
```
powershell "Set-Item -Path Env:NOPROMPT_INSTALL -Value 'true'; IEX(New-Object Net.WebClient).downloadString('https://platform.activestate.com/dl/cli/install.ps1')" && state activate --path %APPDATA%/ActiveState-Recipes/recipe-/580787-implementing-function-based-callbacks-in-python ActiveState-Recipes/recipe-/580787-implementing-function-based-callbacks-in-python
```

macOS: not yet supported

[State Tool]: https://www.activestate.com/products/platform/state-tool/