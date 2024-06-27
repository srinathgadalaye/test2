<h1>Workflows & Events Deep Dive</h1>

<img width="794" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/5c809fee-a737-485f-a4cf-90c83ec3a8c5">
  
  - Official doc of Events that trigger worflow: https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows

- This Will trigger the worflow if there is
  - "push on any branch or anywhere in the repo.." and
  - also "using workflow dispatch we can trigger the worflow through the button"
  ![image](https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/44be287f-4dea-488a-a8d9-7fdea0351101)

</br>
</br>
</br>
<h2> Event Filters and Activity types</h2>
  <img width="872" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/f819c3ed-6050-4337-bb86-61cb5aada875">


</br>
</br>
<h3> Activity Types</h3>
  <img width="917" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/df73dbf5-92eb-4f24-999f-cec492b3b0ff">
  
  - Link to the above screen shot: https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#pull_request
  - By default "pull request" activity type triggers when, activity is "opened", "synchronised" or "reopened".
    
  - Example of Activity type, using for "pull request" - which shows that the workflow will trigger only when an "Open PR request is raised"

    <img width="187" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/fe9897c2-8e9b-4f24-a2f3-911db1fe46a8">


</br>
</br>
<h3>Event Filters</h3>

  ![image](https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/a932e0e1-df49-4b2b-80b9-201b8cc7639c)

  - We can triggere event filter on "push" by the following filters as underlined above:
      - branches
      - tags
      - branch-ignore
      - Tag-ignore
        
  - Example of Event trigger:
    
    <img width="698" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/a7712c3e-9b34-4fd2-9d67-b0171a5bbb82">

  - Another examples of adding event triggers(the branches part of "pull request"):

    <img width="662" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/3238cc25-a83e-4adc-882d-ba2e06303eef">


  
- Offical doc to learn about Event filters: https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions
- Filter Pattern Cheat Sheet: https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#filter-pattern-cheat-sheet


</br>
</br>
<h3>Final Github worflow code: Having Events filters and activity type asper above exmaples </h3>

  ![image](https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/16741e1a-a9d9-42ab-a98a-73880ab1e6b6)

  
  - Link to the worflow: https://github.com/BaliDataMan/github-actions-course-resources/blob/main/Code/03%20Events/02%20Finished%20Project/.github/workflows/demo1.yml


</br>
</br>
</br>
<h2> Special Behaviour: Forks & Pull Request Events</h2>

  <img width="870" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/32915547-3d22-4485-a5b7-495c9f8c175d">

  - If its added as Contributor the flow will excute, but if someone unknown or first time raising PR, the Github worflow will not execute even if the PR is asper the code written in Github worflows.


</br>
</br>
</br>
<h2> Cancelling and Skipping the Workflow</h2>

  <img width="837" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/a2e67a8f-535b-412b-904c-eef10eb6a594">



- You can Manually cancel the worflow through the button as shown with yellow circle below:
    
  <img width="923" alt="Screenshot 2024-06-27 at 5 59 23 PM" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/03cf1a9f-3b55-4583-97c1-f2ff9a7c695c">

- You can skip workflow runs triggered by the push and pull_request events by including a command in your commit message.


  - Example of skipping the worflow:
  
      <img width="404" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/1825de60-8d33-4113-b5fe-94809c803488">

    
  - For more details (official doc: https://docs.github.com/en/actions/managing-workflow-runs/skipping-workflow-runs):

      <img width="676" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/97736291-5f6c-4512-8552-c1dd6c059146">



</br>
</br>
</br>
<h2> Summary</h2>

  <img width="1104" alt="image" src="https://github.com/BaliDataMan/github-actions-course-resources/assets/29046663/12672300-aa0a-4f53-a5d5-42061d455fcc">


  
