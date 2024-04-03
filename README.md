# Pass in web
Project made during the Next Level Week led by [Diego Fernandes](https://github.com/diego3g) from [Rocketseat](https://www.rocketseat.com.br) team between 01/04/2024 and 05/04/2024.

# How to run (in windows)
> *A pull request with others OS instructions is very welcomed.*

This [React](https://react.dev/) project is made using [Vite](https://vitejs.dev) (v5.2.3) and [Typescript](https://www.typescriptlang.org/).  
Vite itself is run by [Node Package Manager (NPM)](https://nodejs.org/en).  

### Setup Node.js
> - *using version 20.12.1*
> - *all commands were run in Windows PowerShell as administrator*

Before run the project you need Node.js. If you already have it, skip this step.

Personally, I'm prefer to use Chocolatey to install and maintain Node.js but you can install it however you prefer.

To install Chocolatey, run:
```
Set-ExecutionPolicy Bypass -Scope Process -Force;
[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072;
iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'));
```

When I created this project, Chocolatey had not the 20.12.1 (LTS) node version, so I used this command to install node.js:
```
choco install nodejs-lts
```

But in your case, you can specifically download the 20.12.1 node version using:
```
choco install nodejs --version="20.12.1"
```