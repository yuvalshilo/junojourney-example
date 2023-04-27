# junojourney-example
Simple example showing manual testing a PR check status 

## Setup
Using a temporary workaround to enable `check` for a Repo only publishing **Manual** tests results in Testspace.

- Add a simple GitHub workflow to publish 1-time only. Note, this workflow has to be in the master (default) branch before any other working branches use it.

Also need to setup the `.testspace.yml` file:

```
manual:
  issues: 
  provider: generic  # If not using GitHub 

release:
  - "*"
```

