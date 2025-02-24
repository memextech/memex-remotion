# Remotion Starter Project

This templates spins up Remotion, which can be used to create dynamic videos with React 19 and TypeScript.  

It includes two starter compositions: **HelloWorld** and **OnlyLogo**.

After it's set up, you can ask Memex in natural language to generate visualizations, and it will generate composition files for you without needing to know how to code them!


## Potential app functionality expansions to explore

Here are some ideas of visualizations you can ask Memex to generate for you once the project is up and running:
- Generate an animation of a red square that bounces around the screen
- Generate an animation of a logo and the following text: "Logo"


## Quick Start

Just ask Memex to run this app locally and it will take care of the rest! If you run into any errors, just point Memex to fix them.

If you’d like to set up the environment and dependencies manually, follow the steps at the bottom of this page.

## Development

See Rules for AI (rendered from .memex/rules.md) for detailed development guidelines Memex will follow, including:
- Complete setup instructions
- Model-specific parameters
- Error handling
- Potential improvements
- Development workflow

You can ask Memex to update rules.md to reflect your project needs as you expand it, or set it as part of your Custom Instructions so that it does it automatically after important steps.

----

### Installation


Use your preferred package manager (like bun) to install dependencies. For example:

```bash
bun install
```

### Scripts

#### dev
- **Command**: `remotion studio`  
- **Description**: Starts the Remotion Studio on [http://localhost:3000/](http://localhost:3000/)

#### build
- **Command**: `remotion render`  
- **Description**: Builds and renders the video to an output folder

#### upgrade
- **Command**: `remotion upgrade`  
- **Description**: Upgrades Remotion to the latest version

#### test
- **Command**: `eslint src && tsc`  
- **Description**: Runs ESLint and TypeScript checks

---

## Usage

### Compositions

#### HelloWorld
- **Description**: Demonstrates an animated title, subtitle, and a rotating color-changing logo.  
- **Default Props**:  
  - `titleText`: **Welcome to Remotion**  
  - `titleColor`: **#000000**  
  - `logoColor1`: **#91EAE4**  
  - `logoColor2`: **#86A8E7**  

To preview it, run the `dev` script and select **HelloWorld**.

#### OnlyLogo
- **Description**: Renders only the rotating color-changing logo with two gradient arcs.  
- **Default Props**:  
  - `logoColor1`: **#91dAE2**  
  - `logoColor2`: **#86A8E7**  

---

## Notes

- The source code is in `src/`. Look at `HelloWorld.tsx` for the composite example that includes the "Title", "Subtitle", and "Logo" components.
- `Logo.tsx` and `Arc.tsx` demonstrate using Remotion hooks like [`useVideoConfig`](https://www.remotion.dev/docs/use-video-config) and [`useCurrentFrame`](https://www.remotion.dev/docs/use-current-frame) to add timeline-based animation.
