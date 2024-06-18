## Transpile-only doesn't work without tsconfig.json

```bash
node -r ts-node/register src/app.ts - ok
node -r ts-node/register/transpile-only src/app.ts - error TS5109
```

If you copy tsconfig.json from src to the app root there will be no error.
