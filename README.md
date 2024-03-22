1. `pnpm install`
2. `pnpm exec turbo build`
    - config.json is first created by build-config-file
3. `rm ./apps/app-1/config.json`
    - simulate the repo's initial state
4. `pnpm exec turbo build`
    - shows first's config.json contents even though config.json is listed in inputs & has changed.
      this should be a cache miss.
