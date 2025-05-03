# assistant_prompts


This repository stores the production‑ready prompt libraries for the **SmartBusinessExpert** multi‑agent stack.

## Structure
```
assistant_prompts/
├── AI-Project-Manager-Assistant.json   # Main PM agent prompt (auto‑generated)
├── .github/workflows/ci.yml            # Smoke‑tests + JSON lint
├── .gitignore
└── README.md
```

### Usage
1. Clone the repo  
   ```bash
   git clone <your‑repo‑url>.git
   ```
2. Edit prompts locally, commit, push.  
3. The CI workflow lints JSON and deploys to **Make** via REST API.

### CI Notes
* The workflow is intentionally minimal – adjust for your infra.
* Secrets required:
  * `MAKE_WEBHOOK_URL`
  * `MAKE_TOKEN`

© 2025 SmartBusinessExpert
