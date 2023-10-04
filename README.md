# LEVEL


## Project Website
[LEVEL Platform](https://shivangraikar.github.io/LEVEL/)

## Introduction
The goal of this project is to provide standardized visualization benchmark datasets
and rankings of computational methods for visualization understanding.

The users can train their models and submit a pull request which triggers the GitHub Action workflow, 
run the script remotely in the school server, compute the scores, and update the website leaderboard accordingly.

## Technologies
- **HTML + CSS + JavaScript**: Provide the structure, interactivity and behavior of our website.
- **Python**: Evaluates the training model and merge the results into the database. 
- **Miniconda**: Ensures that the Python files run smoothly and conflict-free on the server side.
- **AJAX**: Allows for dynamic content updates, improving user experience.
- **GitHub Workflow**: Automates the process directly in the GitHub repository. 
- **GitHub Pages + Jekyll**: Streamline the hosting and support of our static website, ensuring the leaderboard remains updated.

## Submit
- Fork the repository
- Train your CQAW data
- Submit a pull request

After the pull request is accepted, the evaluation will run under the hood (you can check the Github Action for the process).
Once the evaluation is done, refresh the page. The leaderboard will be ranked based on the quality of prediction.


Please remember that published.lock in the remote server will prevent the workflow from triggering (**remove** it before accept the pull request).

The following in the GitHub Action indicates that the published.lock is presented in the server.
```
out: Script already executed. Skipping script execution.
```
See publish.yml for more information about the workflow.

## Make sure you have ruby installed before host our website on the local machine
In the terminal you can check the ruby and gem version by running
```
ruby -v
```
and
```
gem -v
```
## You can host the website locally by running
```
jekyll s
```
You will see the following, click the **Server address** to open up the website
```
Configuration file: /Users/woodylin/Documents/LEVEL/_config.yml
            Source: /Users/woodylin/Documents/LEVEL
       Destination: /Users/woodylin/Documents/LEVEL/_site
 Incremental build: disabled. Enable with --incremental
      Generating... 
                    done in 0.249 seconds.
 Auto-regeneration: enabled for '/Users/shivangraikar/Desktop/LEVEL'
    Server address: http://127.0.0.1:4000
  Server running... press ctrl-c to stop.
```

## Limitation
The website is currently in beta. It's designated to test out the GitHub workflow for CQAW challenge right now. If you wish to modify the website
for your own sake, feel free to do that. You can add more functionality and features.

## Licence 
MIT