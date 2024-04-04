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

### Clone this project
```
git clone https://github.com/MDIVS/nlw-2024-pass-in-web.git # clone this repo

cd nlw-2024-pass-in-web # access project folder

npm i # install dependencies
```

### Running
Now you problably are ready to go with
```
npm run dev
```

# How was it made
### Getting ready
To create a new project, just type
```
npm create vite@latest
```

Enter the `Project Name`, then select `React` and `TypeScript`.

This will create the project in the folder with the specified project name. Now you can open the folder and install dependencies.

```
cd <PROJECT_NAME>
npm i
```

### Tailwind
We are using [Tailwind](https://tailwindcss.com/) here to improve stylization productivity. To install tailwind in a Vite project follow [this tutorial](https://tailwindcss.com/docs/guides/vite).

Also, if using VS Code, it is recommended to install the [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss) extension.

After installing Tailwind, execute this Tailwind Merge installation for easily merge styles:
```
npm i tailwind-merge
```

### Lucide React
Icons, icons and more icons (IN SVG!!!!!!)
```
npm i lucide-react
```

### Faker
Used to fake database data allowing us to test our project before connect it into an api.

Install it as a Dev Dependency.
```
npm install @faker-js/faker --save-dev
```

### Dayjs
Used to handle data with localization.

Install it by running:
```
npm i dayjs
```