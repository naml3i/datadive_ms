# datadive_ms
A repo for the ML Forecasting DataDive of the Münster Data Science Meetup

This is hafenjungs knowledge sharing repo to tackle the [Swimming Pool Visitor Forecast Competition](https://inclass.kaggle.com/c/swimming-pool-visitor-forecasting) in Münster, October 29-30 2016.


## Working with Branches

Avoid committing directly to the `master` branch!

Branches are useful to contribute to a central repository, by using the pull request workflow. The following is a (very basic) introduction on how to create a branch, work on a feature, push changes to the branch and finally clean after yourself.

Follow these steps for a simple but efficient workflow.

#### Create a branch and track remote

- Checkout a new branch (e.g called review) `git checkout -b review`
- Push branch to track remote `git push --set-upstream origin review`
- To move to the `review` or `master` branch: `git fetch && git checkout review` or `master` to make changes.

#### Create a Pull Request

- Go to your github repository. Click on the create pull request tab.
- Select which branch you would like to track changes against master (if you used the above nomenclature, it would be `review`).
- Pull requests should be clear, contain tests. notify other contributors of your pull request.
- Important: Don't merge your pull requests until they have been reviewed!

#### Deleting an unnecesary branch

- Remember to check out all changes first. Then, move to the master branch: `git fetch && git checkout master`.
- Delete old review branch: locally `git branch -D review` and in origin `git push --delete origin review`
