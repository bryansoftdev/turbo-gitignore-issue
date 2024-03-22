1. pnpm install
2. pnpm exec turbo build
    - config.json is created
3. rm config.json
4. pnpm exec turbo build
    - Shows old config.json contents even though it config.json listed in inputs & has changed
