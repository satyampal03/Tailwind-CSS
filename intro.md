# 🧩 Tailwind CSS – Complete

## What is Tailwind CSS?

> - Tailwind CSS is the *CSS framework*, In which we use the the direct CSS in the HTML File, we don't need to write CSS-Code in external even in head of the page.

>> - **It is faster then external file code**
>> - **No className headache**


# TO INSTALL TAILWIND 

> npm init -y  
> npm install -D tailwindcss  (-D  => This istall as the DEV Dependencies -- that can be use at development face)    when we deploye our application then this will not overhide lot, (tailwind css dependencies will install including node-modules folder)

```Tailwind CSS works by scanning all of your HTML files, JavaScript components, and any other templates for class names, generating the corresponding styles and then writing them to a static CSS file.```


## Install NPM 
 1. To Install all dependencies of Tailwind-CSS <br>

 ``` npm install -D tailwindcss```

2. To install  post css file in our code 
<br>

```npx tailwindcss -p```

3. To get the tailwind.config.js file
<br>

```In v-4 of node.js npx tailwindcss init commond being removed and now we hava to create it manualy or there is one another way ```<br>

```create the file manually ---> tailwind.config.js```


#### Manually paste this line into our tailwind.config file

##### This file only use when we want to costumise our tailwind css file.

/** @type {import('tailwindcss').Config} */
export default {
  content: ["./*.html"], // these files will check in the project in react we also include the .js file to be watch but in tailwind css we do not include the js file.
  theme: {
    extend: {},
  },
  plugins: [],
};

#### This command will scan or watch  all of the components of our project that all that we have included in the tailwind-config file.

```npx @tailwindcss/cli -i ./src/input.css -o ./dist/output.css --watch```



- 1️⃣Which files to scan for tools you are 
 actually using

- 2️⃣ What extra tools you want to add
- 3️⃣ Any plugins you want to include

```This config file will work with only the needed file.```

## How to setup Tailwind-CSS

- Create the Folder of your project. 
 ```my_project```

- Installation with CLI
 ```Tailwind CLI";```

- Install Tailwind CSS
 ```npm install tailwindcss @tailwindcss/cli => this cmd will generate the 3 file or folders node_modeles, package-lock.json, package.json```  


- Import Tailwind in your CSS
``` create src folder in that create the input.css file, src/input.css --> @import "tailwindcss" ```

- Start the Tailwind CLI build process
``` npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch```


- Start using Tailwind in your HTML
``` now create the html file in root of the Project index.html```

```now link the outer.css file in the html head```