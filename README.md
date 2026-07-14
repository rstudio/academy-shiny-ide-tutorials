# Posit Academy — Shiny IDE Tutorial Files

Starter files for Posit Academy Shiny for R IDE tutorials. These tutorials run in your browser but ask you to work with files in your IDE (Positron or RStudio) alongside the tutorial.

**By accessing these Posit Academy course materials, you agree to Posit's [End User License Agreement](https://posit.co/about/eula/) and [Learning Services Agreement](https://posit.co/learning-services-agreement/).**

## Setup

Clone this repository in a Terminal on Posit Workbench:

```bash
git clone https://github.com/rstudio/academy-shiny-ide-tutorials.git
```

## Folder contents

| Folder | Starter Files | Tutorial |
|--------|---------------|----------|
| `01-shiny-welcome_to_shiny/` | `ex01.R` | Welcome to Shiny: your first app, UI & layouts, input widgets |
| `02-shiny-basics_of_reactivity/` | `ex01.R`, `ex02.R`, `ex03.R` | Basics of reactivity: outputs, the server function, the reactive graph |
| `03-shiny-more_reactivity/` | `ex01.R`, `ex02.R`, `ex03.R` | More reactivity: `reactive()`, `observe()`, `req()`, and `bindEvent()` |
| `04-shiny-dynamic_modern_ui/` | `ex01.R`, `ex02.R`, `ex03.R` | Dynamic and modern UIs: bslib cards, value boxes, and `renderUI()` |
| `05-shiny-customization_and_theming/` | `bslib.R`, `shiny.R`, `colors.R`, `darkmode.R` | Customization and theming: Bootstrap versions, `bs_theme()`, dark mode, thematic |
| `06-shiny-workflow_and_deployment/` | `app.R` | Workflow and deployment: organizing an app and publishing to Posit Connect Cloud |
| `07-shiny-more_interactive_visualizations/` | `leaflet.R`, `plotly.R`, `dt.R` | More interactive visualizations: leaflet maps, plotly plots, DT tables (optional) |
| `08-shiny-production_ready_apps/` | `testing.R`, `app.R` | Production-ready apps: testing with shinytest2 (optional) |
| `09-shiny-user_input_validation/` | `validation.R`, `feedback.R` | User input & validation: `req()`, `validate()`, and user feedback (optional) |

Each folder contains the starter `.R` app file(s) and the `data/` files needed for that tutorial.

## How to use

When a tutorial asks you to open a starter file, navigate to the corresponding folder and open the `.R` file in your IDE. To run an app:

- **RStudio**: click the **Run App** button in the editor toolbar.
- **Positron**: run the app from the Console with a lesson-folder-qualified path, e.g.

  ```r
  shiny::runApp("01-shiny-welcome_to_shiny/ex01.R")
  ```

This works from the repo root: `runApp()` temporarily switches to the app's folder while the app runs, so the app can find its `data/` files. (Avoid an argument-less `shiny::runApp()` — from the repo root it cannot find the app or its data.)
