<h1>Workflows & Events Deep Dive</h1>

<img width="794" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/5c809fee-a737-485f-a4cf-90c83ec3a8c5">
  
  - Official doc of Events that trigger worflow: https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows

- This Will trigger the worflow if there is
  - "push on any branch or anywhere in the repo.." and
  - also "using workflow dispatch we can trigger the worflow through the button"
  ![image](https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/44be287f-4dea-488a-a8d9-7fdea0351101)


<h2> Event Filters and Activity types</h2>
  <img width="872" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/f819c3ed-6050-4337-bb86-61cb5aada875">

<h3> Activity Types</h3>
  <img width="917" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/df73dbf5-92eb-4f24-999f-cec492b3b0ff">
  
  - Link to the above screen shot: https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#pull_request
  - By default "pull request" activity type triggers when, activity is "opened", "synchronised" or "reopened".
    
  - Example of Activity type, using for "pull request" - which shows that the workflow will trigger only when an "Open PR request is raised"

    <img width="187" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/fe9897c2-8e9b-4f24-a2f3-911db1fe46a8">

  
<h3>Event Filters</h3>

- Filter Pattern Cheat Sheet: https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#filter-pattern-cheat-sheet

<h2>Final Github actions having Events</h2>
  
  - Link to the worflow: https://github.com/BaliDataMan/github-actions-course-resources/blob/main/Code/03%20Events/02%20Finished%20Project/.github/workflows/demo1.yml 
