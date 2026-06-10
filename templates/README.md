# Module Curriculum Templates

This folder contains reusable templates for creating new module curriculum material. Each template mirrors the file and folder structure used in `Workshops/Module1/` through `Workshops/Module5/`.

## Recommended: Use the Module Curriculum Skill

The `.github/skills/module-curriculum/` skill automates the steps below. Ask GitHub Copilot to "add a new module" and it will read these templates, fill the placeholders, and update the root `README.md`. See [`.github/skills/module-curriculum/SKILL.md`](../.github/skills/module-curriculum/SKILL.md).

## How to Use (manual)

1. **Copy** the templates into a new folder, e.g. `Workshops/Module5/`.
2. **Rename** each file following the numbering convention: `{N}-{Topic-Name}.md`.
3. **Replace** every `{{PLACEHOLDER}}` with the appropriate value for the new module.
4. **Use** the lab template for the lab page:
   - [LAB-SKILLS-TEMPLATE.md](LAB-SKILLS-TEMPLATE.md), all labs in this curriculum link to an external GitHub Skills exercise at `github.com/skills/`. Do not compose inline lab exercises.
5. **Update** the root `README.md` using the snippet in [README-SNIPPET.md](README-SNIPPET.md).

## Folder Structure After Copying

```text
Workshops/Module{{MODULE_NUMBER}}/
├── 1-{{SESSION_1_TOPIC}}.md          ← from SESSION-TEMPLATE.md
├── 2-{{SESSION_2_TOPIC}}.md          ← from SESSION-TEMPLATE.md (duplicate for additional sessions)
├── {{LAB_FILE_NUMBER}}-Module{{MODULE_NUMBER}}-Lab.md  ← from LAB-SKILLS-TEMPLATE.md
└── {{PROMPTS_FILE_NUMBER}}-Module{{MODULE_NUMBER}}-Prompts.md ← from PROMPTS-TEMPLATE.md
```

## Placeholder Reference

| Placeholder | Description | Example |
|---|---|---|
| `{{MODULE_NUMBER}}` | Module number (integer) | `5` |
| `{{MODULE_TITLE}}` | Short title for the module | `Advanced Agent Workflows` |
| `{{MODULE_OBJECTIVE}}` | One-sentence learning objective | `Explore autonomous agent capabilities and multi-step workflows.` |
| `{{MODULE_TOTAL_DURATION}}` | Estimated total hours | `2-3 hours` |
| `{{SESSION_TITLE}}` | H1 heading for a session | `Agent Mode Deep Dive` |
| `{{SESSION_DURATION}}` | Session length | `45-60 minutes` |
| `{{SESSION_OBJECTIVE}}` | Session learning goal | `Understand how Agent Mode orchestrates multi-file changes.` |
| `{{SESSION_CONTENTS}}` | Table of contents entries | See SESSION-TEMPLATE.md |
| `{{SESSION_BODY}}` | Main session content sections | See SESSION-TEMPLATE.md |
| `{{LAB_TITLE}}` | H1 heading for the lab | `Agent Workflows Hands-On Lab` |
| `{{LAB_DURATION}}` | Lab time estimate | `60-90 minutes` |
| `{{LAB_DESCRIPTION}}` | Short lab description | `Build an agent-driven refactoring pipeline.` |
| `{{LAB_FILE_NUMBER}}` | Position in the file list | `3` |
| `{{PROMPTS_FILE_NUMBER}}` | Position in the file list | `4` |
| `{{PROMPTS_OBJECTIVE}}` | Purpose of the prompts page | `Provide reference prompts for agent workflows.` |
| `{{NEXT_SESSION_TITLE}}` | Title of the following page | `Module 5 Prompt Examples` |
| `{{NEXT_SESSION_FILE}}` | Relative path to the next file | `4-Module5-Prompts.md` |
| `{{NEXT_MODULE_SESSION_TITLE}}` | First session of the following module | `Continue to Module 6` |
| `{{NEXT_MODULE_SESSION_FILE}}` | Relative path to that file | `../Module6/1-Topic.md` |
| `{{PREVIOUS_MODULE_NUMBER}}` | Previous module number | `4` |
| `{{PREPARED_REPOSITORY_URL}}` | Prepared workshop repository URL that participants open directly | `https://github.com/martinpolivka/skills-example` |
| `{{SKILLS_REPO_OWNER}}` | GitHub Skills template owner | `skills` |
| `{{SKILLS_REPO_NAME}}` | GitHub Skills template repo name | `getting-started-with-github-copilot` |

## Styling Rules

All new content **must** follow the rules in [`.github/instructions/Currriculum-Styling.instructions.md`](../.github/instructions/Currriculum-Styling.instructions.md):

- British English spelling throughout.
- No emdashes. Use full stops or commas to separate clauses.
- Every page ends with a **Next Steps** section.
- Code blocks include comments explaining purpose and key details.
- Update the root `README.md` date and Table of Contents when adding a module.
