# np-azure-swa
Azure Static Web App Test

Azure Static Web Apps is a fully hosted, serverless system for automated deployment from github repos to a static site. This platform performs well for static site generators and single page web applications

For this first proof-of-concept, I've created a basic text-based site in github which I am looking to setup automated deployment to the static web apps platform. 

It took an initial amount of work to get basic things in place like github repos, local development environments, local software updated, and azure cli installed:
- Created a public repo in github for my project. git@github.com:nathanpedretti/np-azure-swa.git
- Cloned the repo to my local and created some basic content on the 'main' branch. For this POC, I'm not worrying about a build step. I'm focusing on getting a CD pipeline in place to auto deploy changes.
- Updated the version of node and npm on my machine to 18.16.0 and 9.5.1 respectively
- Updated homebrew on my macbook to 4.0.0. This was a requirement as the package manager to pull down the Azure CLI
- After updating homebrew, discovered that I needed to install the xcode-developer tools to support the Azure CLI. These were installed and updated.
- Finally, I was able to 'az login' to my person development azure subscription to begin work.