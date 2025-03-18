# LottoJaxx Website

This repository contains the LottoJaxx website landing page built with HTML, JavaScript, and Tailwind CSS.

## Project Structure

```
lotto-jaxx/
├── public/           # Contains HTML, JS files and compiled CSS
│   ├── index.html
│   ├── output.css    # Compiled Tailwind CSS
│   └── ...other files
├── src/
│   └── input.css     # Tailwind CSS source file
├── tailwind.config.js
└── package.json
```

## Development Setup

### Prerequisites

- Node.js (latest LTS version recommended)
- npm (comes with Node.js)

### Installation

1. Clone this repository:
   ```
   
     git clone <repository-url>

   ```
   ```
   
     cd lotto-jaxx
   
   ```

2. Install dependencies:
   ```
   
     npm install
   
   ```

3. Make sure to install Tailwind CSS:
   ```
    
     npm install -D tailwindcss
   
   ```
   ```
   
     npx tailwindcss init
   
   ```

## Development Workflow

### Start Development Server

To start development with auto-reloading CSS:

```

  npx tailwindcss -i ./src/input.css -o ./public/output.css --watch

```

This command will:
- Watch for changes in the `./src/input.css` file
- Process the Tailwind CSS
- Output the compiled CSS to `./public/output.css`
- Continue watching for changes

### Testing the Website

Open the `public/index.html` file in your browser to view the website.

## Building for Production

### Create Production Build

When you're ready to build the website for production:

```

  npx tailwindcss -i ./src/input.css -o ./public/main.css --minify

```

This command will:
- Process the Tailwind CSS
- Minify the output CSS for production
- Write the final CSS to `./public/output.css`

### Deploying the Website

1. After running the production build command, you need to package your website files.

2. Create a zip archive of the `public` folder:
   ```
   # On Linux/Mac
   zip -r lotto-jaxx.zip public/
   
   # On Windows
   # Right-click the public folder -> Send to -> Compressed (zipped) folder
   ```

3. The resulting `lotto-jaxx.zip` file contains everything needed to deploy your website.

## Maintenance

To update Tailwind CSS or other dependencies:

```

  npm update

```

