# Guidelines for an LLM-Powered Agent Developer

Welcome to the **memex-remotion** project! These rules are for an LLM-powered agent developer looking to enhance, optimize, or contribute new features to this codebase.

---

## 1. Overview

- **Project Purpose**: This repository creates dynamic videos using [Remotion](https://www.remotion.dev/docs), React 19, and TypeScript.  
- **Code Structure**:
  - `src/`: Core logic for Remotion compositions.
  - `package.json`: Project scripts and dependencies.
  - `README.md`: General installation and usage guide.

---

## 2. Environment Setup

1. **Dependencies**: Follow the instructions in [README.md](../README.md) to install and manage dependencies.  
2. **Running the Project**:  
   - Use `bun install` to ensure all packages are installed.  
   - Run `bun dev` or `remotion studio` to open Remotion Studio for previews.  
   - Build with `remotion render` to create final outputs.

---

## 3. Coding Standards

1. **Language & Frameworks**:  
   - Use React 19, TypeScript, and the latest Remotion API.  
   - Maintain high code quality (lint, type-check, etc.).  
2. **Styling & Conventions**:  
   - Follow ESLint rules as configured in the project.  
   - Use Prettier for consistent formatting (see `.prettierrc` if applicable).  
3. **Directory Structure**:  
   - Keep core logic in the existing `src/HelloWorld/` folder unless otherwise needed.  
   - Keep components modular and composable.  

---

## 4. Contribution Workflow

1. **Branching**: Create feature-specific or fix-specific branches for all changes.  
2. **Commits**: Use clear, concise commit messages to describe work in progress.  
3. **Pull Requests**:  
   - Ensure lint checks and type checks pass.  
   - Provide a clear description of the feature, fix, or enhancement.  
4. **Reviews**: Another contributor or a maintainer must review your PR. Address feedback quickly and keep the conversation constructive.

---

## 5. Testing

- Use the existing scripts (`test`) to run ESLint and TypeScript checks.  
- Ensure that new or changed compositions render as expected in Remotion Studio.  
- Validate the final output with `remotion render` when introducing significant changes to the code structure.

---

## 6. LLM-Powered Workflows

- **Automated Code Suggestions**:  
  - May be used but must be reviewed thoroughly for correctness.  
- **Documentation**:  
  - If your LLM outputs updated docs or instructions, ensure they are accurate and do not contradict existing documentation or code comments.

---

## 7. Deployment & Production

- **Build Process**: Rely on `remotion render` to generate final videos.  
- **Production Considerations**:
  - Keep library versions aligned (see `package.json`)  
  - Watch for potential performance bottlenecks in video rendering (in case of heavy composition logic).  

---

## 8. Support & Feedback

- For questions, open an issue or talk to a project maintainer.
- If an LLM is used for code assistance, double-check the recommended changes for accuracy.

---

**Thank you for contributing to this project!**
