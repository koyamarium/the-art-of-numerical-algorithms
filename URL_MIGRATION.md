# Legacy Pages redirect

The atlas now lives at https://koyamarium.github.io/numerical-methods-atlas/ .
`legacy-site/` contains only the redirect entry, 404 fallback and route-preserving module. The Pages workflow checks the new site's metadata before replacing the old distribution.

The original Python sources, commit history, tags and v0.1.0 release remain here. The prior deployed source is `e5b93f4a01e94f0a44ac34004e8db22f6335bbfc`. To restore the prior site, create a new commit restoring `.github/workflows/pages.yml` and `website/` from that commit, then run its Pages workflow. Do not reset or delete the history.

The local migration operator also retains a Git bundle and a rebuilt legacy static distribution under `outputs/migration-rollback/` in the development checkout.
