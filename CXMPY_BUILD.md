# Cxmpy Apps build

This repository contains the Cxmpy Apps branding changes and a GitHub Actions workflow that builds the Nintendo Switch `.nro`.

## Build without installing devkitPro locally

1. Create a new GitHub repository and upload this project, including the `.gitmodules` file.
2. Make sure the repository contains the `.github/workflows/build-cxmpy-apps.yml` workflow.
3. Open **Actions → Build Cxmpy Apps NRO → Run workflow**.
4. When the job finishes, open the workflow run and download the **CxmpyApps** artifact.
5. Extract `CxmpyApps.nro` and copy it to `sd:/switch/` on the Switch SD card.

The workflow checks out the project's git submodules recursively because the build depends on vendored submodules.
