# DotNET-Core-Playground
Testing webshells and the like with MVC and Dot NET Core

## Using the webshell
The webshell itself is `/Views/Home/Shell.cshtml`. You can play with it as well by selecting `Sh3ll` on the top menu of this solution.

You can also find the webshell itself in a different repo: https://github.com/auseche-r7/DotNET-Core-Shell

## LFI Sample
The home page allows you to test LFI with the webshell. I will be adding demos for RFI as well soon.

To get the LFI working the url should look something like this

`http://localhost:63425/Home?tpl=~/Views/Home/Shell.cshtml&cmd=ls`

The above simulates a web page that pulls a partial view from `~/Views/Home/Shell.cshtml`. You can simply enter `http://localhost:63425/Home?tpl=~/Views/Home/Shell.cshtml` and ommit the `cmd` argument, as it will be added for you when entering commands in the shell.

## RFI Sample 

In progress
