# Mechanical Keyboard Simulator - [kbs.im](https://kbs.im)
![kbs.im picture](https://github.com/tplai/kbsim/blob/master/src/assets/images/demo.PNG)

Mechanical Keyboard Simulator is website that simulates typing on a variety of custom keyswitches and offers a simple typing test. Currently, it supports 10+ switches, keyboard layouts, and colors for an customizable, satisfying typing experience.

## Features
- Unique sounds for specific keys
- 1 minute English typing test
- Wide selection of case colors and layouts
- Dark mode

## Currently Supported Switches
- NovelKeys Creams
- Holy Pandas
- Turqoise Tealios
- Gateron Black Inks
- Cherry MX Blacks
- Cherry MX Browns
- Cherry MX Blues
- Kailh Box Navies
- Buckling Spring
- SKCM Blue Alps
- Topre

## Currently Supported Layouts
- Fullsize
- Tenkeyless
- 75%
- 65%
- HHKB

## Requests
Switch and layout requests are open at the moment, feel free to open an issue if you'd like to see a switch or layout added!

# Developers

## Setup
To run this application locally, use:

```bash
npm install
npm start
```

## Project structure
    .
    ├── src                                           # Source files
    │   ├── assets                                    # audio and image assets
    |   |   ├── audio  
    |   |   └── images
    │   ├── features                                  # components and modules
    │   |   ├── Store                                 # Redux store
    |   |   |   └── store.js
    |   |   └── sampleComponent                       # component structure
    |   |       ├── SampleComponent.js
    |   |       ├── SampleComponentSlice.js
    |   |       └── SampleComponent.module.css
    │   ├── public                                    # robots.txt
    |   |   └── robots.txt
    |   ├── App.test.js                               # starter React test file
    |   ├── index.css                                 # index styling
    |   ├── index.html                                # meta tags
    |   ├── index.js                                  # React entry point
    |   └── serviceWorker.js                          # basic offline usage serviceWorker
    ├── .babelrc                                      # babel transpiler config
    ├── LICENSE.md                                    # MIT license
    ├── README.md                                     # you're reading this!
    ├── package.lock.json                             # npm dependency lockfile
    ├── package.json                                  # dependency file
    ├── webpack.config.json                           # webpack config file
    └── yarn.lock                                     # yarn dependency lockfile

## Deployment

### Deploying to Vercel

This project is configured for easy deployment to Vercel. Follow these steps:

1. Install the Vercel CLI (optional):
   ```bash
   npm install -g vercel
   ```

2. Deploy using one of these methods:

   **Option 1: Using Vercel CLI**
   ```bash
   # Login to Vercel
   vercel login
   
   # Deploy from your local directory
   vercel
   ```

   **Option 2: Using Vercel Dashboard**
   - Create an account on [vercel.com](https://vercel.com)
   - Import your GitHub repository
   - Vercel will automatically detect the project settings
   - Configure the following settings:
     - Framework Preset: Other
     - Build Command: `npm run build`
     - Output Directory: `build`
     - Install Command: `npm install`

3. Configuration options:
   - Environment Variables: Add any required environment variables in the Vercel dashboard
   - Custom Domain: Set up a custom domain in the Vercel project settings
   - Deployment Branch: Configure which branches trigger deployments

The project includes a `vercel.json` configuration file that handles routing and build settings.

## Contributing
Pull requests are welcome, but please do create an issue to discuss any major changes.
