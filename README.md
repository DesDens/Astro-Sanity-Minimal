# Astro Sanity Minimal Starter

## [Demo Site](https://astro-sanity-minimal-starter.netlify.app/)

If you haven't heard about [Astro](https://astro.build) yet you're missing out. This starter repo gives you a blog website with a headless CMS setup using [Sanity.io](https://sanity.io).

Don't be fooled by the simplicity of this starter either. With excellent SEO built in, Astro's excellent developer environment, and performance best practices you're getting one of the best foundations for a personal blog with posts written in markdown. The reason for making such a bare bones starter in terms of styles is that it has what you need out of the box for SEO and site structure but it makes no assumptions about how you want it look and behave. 

Sometimes starters can feel like they are giving us way too much and you'll spend a day picking apart half of the code to get to the setup you actually wanted. Want to use vanilla CSS instead of Tailwind or Scss? No problem!

## Features

- A customizable headless CMS with [Sanity.io](https://sanity.io)
- Excellent SEO Built In
  - Open Graph Tags (Twitter, Facebook, etc.)
  - User Declared Canonical URLs
  - RSS Feed
  - XML Sitemap
  - Robots.txt
  - JSON LD Schema
- Extremely minimal styles
- Performant Google Fonts Setup

## Get Started

Watch my [step-by-step tutorial on YouTube](https://youtu.be/-jAWLTfsSQw)

**Or** 


Follow the manual steps below:

### Initial Sanity Setup

1. [Create a repo from this template](https://github.com/jaydanurwin/astro-sanity-minimal-starter/generate)

Start by setting up the Sanity Studio using node package manager. To set up, run:

npm create sanity@latest

You'll be asked to create an account with your Google or Github login, or you can choose to log in with a dedicated email and password. Afterward, you can create a new project, where you'll be asked to choose a project template. Select the blog schema template. First, though, you'll need to give your project and dataset a name (you can add more datasets if you need one for testing) and choose the path to your studio folder (let's pick studio). You can also choose if you want to use TypeScript and which package manager to use.

√ Fetching existing projects
? Select project to use studio-test [projectID]
? Select dataset to use production
? Project output path: H:\Astro JS Projects\astro-sanity-minimal-starter-main\studio-test
? Select project template Blog (schema)
? Do you want to use TypeScript? No
√ Bootstrapping files from template
√ Resolving latest module versions
√ Creating default project files
? Package manager to use for installing dependencies? npm

2. If you don't have the Sanity CLI already run `npm install -g @sanity/cli`
3. Open a terminal from root folder of the project or open the newly creatd sanity folder in Windows/Mac.

8. Replace the PUBLIC_SANITY_PROJECT_ID value with your token ID

**Note:** You will want to add http://localhost:3000 to your allowed CORS orgins in your Sanity project settings at [https://manage.sanity.io](https://manage.sanity.io)
 
### To run your Sanity Studio

1. Open a terminal located at the sanity folder
2. `sanity install`
3. `sanity start`
4. Your studio should be running on [http://localhost:3333](http://localhost:3333)
5.  Open [http://localhost:3333](http://localhost:3333) and copy the project ID from the Project info section

### To run your Astro site

1.  Open a terminal(or go inside the actual folder itseld and run in cmd: "code ." in VS code) located at the astro folder
2.  `npm install astro`
3.  `npm start`
4.  Your Astro site should be running on [http://localhost:3000](http://localhost:3000)
5.  `npm run build` to build to production locally

IMPORTANT: To add or update posts you NEED to restart the astro site:
Ctrl+C in cmd to terminate the current state and redo npm run dev/npm start
