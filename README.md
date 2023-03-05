
# Terraform nonadmin installation
In the powershell please enter below commands 

--> Set-ExecutionPolicy Bypass -Scope Process -Force;

--> $env:chocolateyUseWindowsCompression='true' ; $env:ChocolateyInstall="$home\choco" ; iwr https://chocolatey.org/install.ps1 -UseBasicParsing | iex ; $env:Path = [System.Environment]::GetEnvironmentVariable("Path","Machine") + ";" + [System.Environment]::GetEnvironmentVariable("Path","User") ; choco --version

--> choco upgrade chocolatey

--> choco install terraform
