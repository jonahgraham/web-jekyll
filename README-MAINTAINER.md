# Maintainer info

TODO: document how to maintain this site and update the Eclipse hosted web.

- https://eclipse-embed-cdt.github.io/
- https://eclipse-embed-cdt.github.io/web-preview/

## Travis

- https://travis-ci.com/github/eclipse-embed-cdt/web-jekyll

## Quick copy/paste

```
bundle exec jekyll serve --trace --safe --baseurl "/web-preview"`

bundle exec jekyll serve --trace --safe

bundle exec jekyll build

bundle exec htmlproofer --allow-hash-href --url-swap \^/web-preview/\:/ ./_site_local

bundle exec htmlproofer --allow-hash-href --url-swap \^/web-preview/\:/ --url-ignore /github.com/xpack/xpack.github.io/blob/master/ ./_site_local

bundle exec htmlproofer --allow-hash-href ./_site_local

bundle exec htmlproofer --allow-hash-href --http_status_ignore=429 ./_site_local

# No longer needed, done automatically by last_modified_at.
bash scripts/adjust-timestamps.sh
```
