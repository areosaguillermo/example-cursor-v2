### Example Node Express API

Minimal Express API with a health check endpoint and Jest tests.

### Requirements
- Node.js 18+
- npm 9+

### Install
```bash
npm install
```

### Run the API
- Dev (with reload):
```bash
npm run dev
```
- Production start:
```bash
npm start
```

### Health check
- GET `/health` → 

### Tests
- Run tests once:
```bash
npm test
```
- Watch mode:
```bash
npm run test:watch
```
Notes:
- The project uses ESM. The test script enables Node's --experimental-vm-modules for Jest.

### How to push changes (GitFlow)
1) Create a feature branch from `develop`:
```bash
git checkout develop && git pull
git checkout -b feature/<short-name>
```
2) Make changes and run tests locally:
```bash
npm test
```
3) Commit using Conventional Commits:
```bash
git add .
git commit -m "feat(scope): concise description"
```
4) Push the branch and open a PR targeting `develop`:
```bash
git push -u origin feature/<short-name>
```
Then open a Pull Request from your branch into `develop`.

### Commit style
- Use Conventional Commits (e.g., `feat(api): add users endpoint`, `fix(health): correct status code`).
