## Repository-specific instructions for AI coding agents

This repository is a homework lab (Terraform / AWS) with the primary user-facing document `READMEw6.md` and an `hw6pictures/` folder containing screenshots. Use the README as the single source of truth for expected developer workflows and example commands.

Key facts for edits and PRs
- This is an instructional Terraform homework repo. Primary files/directories:
  - `READMEw6.md` — step-by-step prerequisites and commands (curl check script, terraform init/validate/plan/apply).
  - `hw6pictures/` — image assets referenced from the README (use relative paths like `./hw6pictures/screenshot (2).png`).

Practical guidance for agents
- When asked to add or modify Terraform code, follow the README's local layout: create a project subfolder (the README demonstrates creating a folder and then `touch 0-auth.tf` and `touch 1-main.tf`). If you add Terraform examples, place them under a clearly named folder at repo root (e.g., `oct26/` or `projectname/`) and include `0-auth.tf` and `1-main.tf` as the README demonstrates.
- Preserve image paths. If you update screenshots or add new ones, put PNGs in `hw6pictures/` and update `READMEw6.md` with the relative path. The README uses `./hw6pictures/<name>.png` links — keep that pattern.
- Important: do NOT modify or commit Terraform state or working directories. The README explicitly warns not to modify `.tfstate`, `.terraform.lock.hcl` or the `.terraform` directory. If you see these tracked, flag them and ask the user before making changes.

Commands and developer workflow (explicit from README)
- Use Git Bash on Windows (README guidance). Commands shown in the README:
  - bootstrap/check script: `curl https://raw.githubusercontent.com/aaron-dm-mcdonald/Class7-notes/refs/heads/main/101825/check.sh | bash` (fall-back uses `--ssl-no-revoke` on Windows if needed).
  - terraform lifecycle in project folder: `terraform init`, `terraform validate`, `terraform plan`, `terraform apply`.

Safety and review rules for infra changes
- Never run `terraform apply` (or commit changes that will run it) without explicit user approval. If a requested change will alter real infrastructure, ask for:
  1) the target AWS account/profile to use, and 2) confirmation that the user wants resources created/modified.

Examples to follow
- If adding a new example module for the homework, create `projectname/0-auth.tf` and `projectname/1-main.tf`, add a small README inside that folder explaining the provider configuration and intended result, and add any screenshots to `hw6pictures/`.

When to ask clarifying questions
- If the task implies making infrastructure changes (applying plans), ask which AWS account/profile and whether the run is allowed.
- If the user asks to refactor or reorganize files, confirm the desired target layout (the README demonstrates the student workflow — preserve or document deviations).

Files to inspect first
- `READMEw6.md` (primary).  
- `hw6pictures/` (images used by README).

If you update this file
- Keep entries short and anchored to files listed above. Prefer concrete edits (add a folder, create 0-auth.tf) rather than vague recommendations.

-- End of project-specific guidance --
