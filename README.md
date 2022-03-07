# prepare-npmrc
Saves ExH and Fibricheck npm registries and tokens to the .nmprc files
This action has to be used when it is required to fetch packages from both Fibricheck and ExtraHorizon package managers.

Example how of a step using this action:
```yaml
- name: Prepare npmrc
  uses: QActions/prepare-npmrc@init
  env:
    GITHUB_TOKEN: ${{ secrets.GH_PACKAGES_FULL_READ_ACCESS_TOKEN }}
    NPM_TOKEN: ${{ secrets.NPM_PACKAGES_FULL_READ_ACCESS_TOKEN }}
```
