# Remotion Starter Project

This project uses Remotion to create dynamic videos with React 19 and TypeScript.  
It includes two compositions: **HelloWorld** and **OnlyLogo**.

---

## Installation

Use your preferred package manager (like bun) to install dependencies. For example:

```bash
bun install
```
---

## Scripts

### dev
- **Command**: `remotion studio`  
- **Description**: Starts the Remotion Studio on [http://localhost:3000/](http://localhost:3000/)

### build
- **Command**: `remotion render`  
- **Description**: Builds and renders the video to an output folder

### upgrade
- **Command**: `remotion upgrade`  
- **Description**: Upgrades Remotion to the latest version

### test
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
