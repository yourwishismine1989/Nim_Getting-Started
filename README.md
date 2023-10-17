# Nim_Getting-Started
A quick how to with your first application example

## __install Nim__
 
### Setup Windows (tested on Windows 11 on 09/26/2023)
    C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe (right-click -> Run as administrator)
        Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
        exit (or close Administrator: Windows PowerShell window)
    C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe
        Invoke-RestMethod -Uri get.scoop.sh | Invoke-Expression
        scoop install git
        scoop bucket add extras
        exit (or close Windows PowerShell window)
    C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe (right-click -> Run as administrator)
        scoop install vcredist-aio
        exit (or close Administrator: Windows PowerShell window)
    * C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe
        scoop install nim
        code
            Add the following VSCode extensions to VSCode
                Nim
            close VSCode window
 
## __helloworld.nim__ (tested on Windows 11 on 10/17/2023)
    New-Item -Type File -Name helloworld.nim -Path .\
    code helloworld.nim
    echo "Hello World"
    CTRL-s
    close VSCode window
### the beauty of Nim
##### the following creates an executable (.exe on Windows)
    nim cc .\helloworld.nim
##### the following creates JavaScript that can be run in the browser or node
    nim js .\helloworld.nim