# msa-devops-2020

Website url: https://msa-2020-devops-jock.azurewebsites.net

# Brief Description
This is a react web app that uses the Azure build and release pipeline for continuous deployment for new commits to the `master` and `develop` branch. For the build Azure pipeline I had a trigger in the yaml file to not run a deployment whenever the README.md file is changed.

When the build/release pipeline is triggered:
1. The specified Node.js verison will be installed
2. Build and run the React app
3. If the Master branch was triggered an archive will be created to publish build artifacts.
