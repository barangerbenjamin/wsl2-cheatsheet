Hello and welcome to this WSL2 Cheatsheet.
The goal is to gather here all tips and known issues about WSL2!

# Issues

## Input/Output error

This happens when the hidden `wslhost.exe` is not working. We just need to restart it!

Close all WSL2 tabs.

Open a Powershell tab and run the following command:
```bash
wsl.exe --shutdown
```
Check that your Ubuntu is properly stopped with the command
```bash
wsl -l -v
```

Open a new WSL2 Tab, problem should be fixed.