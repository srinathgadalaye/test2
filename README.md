- Basic Buidling blocks of Github Actions:
<img width="897" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/8a90460d-ba50-4f17-be06-19e33e52f5ad">

- Official Github Actions Doc: https://docs.github.com/en/actions

- On Github Marketplace we have two options: Apps and Actions:
  - Here is Github Action Marketplace : https://github.com/marketplace?type=actions 

- Github Checkout Action:
  - Repo: https://github.com/actions/checkout?tab=readme-ov-file
  - Marketplace: https://github.com/marketplace/actions/checkout

  ```
  jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - name: Get code
        uses: actions/checkout@v3  #"actions/checkout" define the name and "v3" is the version of teh action
                                  #we can also add more parameters to the checkout action with "with" command refer here: https://github.com/marketplace/actions/checkout#usage
  ```

- **Failing and Analysizing Workflows:** To understand any worflow or just to undestand if whats happening underthe worflow, always refer to the logfile of the workflow which is visible after your workflow executes under the "Actions" tab.

<h1> Errors </h1>

1. **Error to push github actions worflow from local to github**:

   To have access to push Github Action workflows from local system to Github you need to have "developer token" which have access to not just repository but also to workflow, which you can create it from here: https://github.com/settings/tokens (if there are other tokens as well remove them for you) and tick the workflow aswell, as shown in below image:

  <img width="662" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/d990802a-ff47-40c2-aedf-8ae9f00fc2a0">


  Now you have createed new token  using which you can push the github workflow to github..
