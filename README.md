# Frontend.live Preview Github Actions

## How to choose the right action
For regular websites with server-based routing you can use `preview.yml` & `pr-preview-link.yml`. For single page applications (SPAs) with client-based routing there's `preview-spa.yml`and `pr-preview-spa.yml`. Notice the following differences:
- The regular preview will be located at frontend.live/REPO_NAME/BRANCH_NAME/index.html, while the SPA one will be located at spa.frontend.live/REPO_NAME/BRANCH_NAME/.
- For the SPA preview, all slashes in the BRANCH_NAME will be replaced with dashes. The branch `feat/test` in the repo `test-repo` will be located at spa.frontend.live/test-repo/feat-test/.