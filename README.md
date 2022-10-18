# Notes about WinDbg

## Installation

### Download and install

Follow the instructions on [this document](https://learn.microsoft.com/en-us/windows-hardware/drivers/debugger/debugger-download-tools).

> If you only need the debugger, make sure to check "Debugging Tools for Windows" only.

### Set up the OS environment.

The program should be installed under the following directory:

```cmd	
cd "%ProgramFiles(x86)%\Windows Kits\"
```

And, more precisely:

```cmd	
SET VERSION=10
cd "%ProgramFiles(x86)%\Windows Kits\%VERSION%\Debuggers"
```

Then, you must select the binary that is suitable for your architecture.

> If you don't know your PC architecture, just execute the following command:
>
>
> ```cmd
> echo %PROCESSOR_ARCHITECTURE%
> AMD64
> ```
>
> And, remember: AMD64 <=> x86
>
> Thus, for my installation, the full path to the debugger executable is:
>
> `"%ProgramFiles(x86)%\Windows Kits\%VERSION%\Debuggers\x86"`
>
> With `VERSION=10`

Now, you can set the `PATH` environment variable so that you can execute the debugger easily.


