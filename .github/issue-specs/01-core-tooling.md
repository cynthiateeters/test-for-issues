---
title: "Core Spec #1: Professional Tooling Setup"
labels: required, setup, week-01, status:todo
---

## 📋 Professional Development Environment

### Requirements (All Must Be Checked)
- [ ] npm installed and package.json created with proper metadata
- [ ] Prettier configured with .prettierrc
- [ ] HTMLHint configured with .htmlhintrc  
- [ ] Stylelint configured with .stylelintrc.json
- [ ] All linting scripts working in package.json
- [ ] .gitignore includes node_modules/

### Verification Commands
Run these commands and paste successful output below:
```bash
npm run format
npm run lint:html
npm run lint:css
```

### package.json Scripts Required
```json
{
  "scripts": {
    "format": "prettier --write .",
    "lint:html": "htmlhint *.html",
    "lint:css": "stylelint **/*.css",
    "lint": "npm run lint:html && npm run lint:css"
  }
}
```

### AI Documentation
- [ ] Created prompt-log.md with setup prompts used
- [ ] Documented any AI-suggested configurations
- [ ] Explained what was modified from AI suggestions

### Status Signal
When complete, change label from `status:todo` to `status:ready-for-review`

---
⚠️ **This is PASS/FAIL** - All boxes must be checked for credit