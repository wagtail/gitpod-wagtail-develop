# Gitpod Wagtail Develop

Develop Wagtail CMS via Gitpod.

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/wagtail/gitpod-wagtail-develop)

Use [wagtail-gitpod](https://github.com/wagtail/wagtail-gitpod) to develop a Wagtail website.

## Steps

1. Click the ``Open in Gitpod`` button.
2. Relax: a development environment with [Wagtail](https://github.com/wagtail/wagtail) and [Bakery Demo](https://github.com/wagtail/bakerydemo) will be created for you.
3. To get to the admin login screen, click on the URL and add `/admin/` at the end. You can login with username: `admin` and password: `changeme`.

By default, the Wagtail bakery demo is opened live once all the assets and dependencies has finished compiling.

More on [contributing and developing](https://docs.wagtail.io/en/stable/contributing/developing.html).

## Contribute to Wagtail

Woo-hoo, you have a working development environment and know how to make a git commit. 
But how do you contribute to Wagtail? 
Here is how to fork Wagtail, create an access token, set a remote, and submit a pull request.

### Fork Wagtail

Go to https://github.com/wagtail/wagtail and click on the Fork button in the top-right corner. 
It creates a new copy of Wagtail repo under your GitHub account. 
The URL will be https://github.com/USERNAME/wagtail

### Create an access token

1. Go to https://github.com/settings/tokens 
2. Click 'Generate new token'
3. Give the token a 'Note' ('Wagtail GitPod' is a good one)
4. If you plan to use this GitPod for more than a month, be sure to choose a longer expiration for the token
5. Tick the checkbox next to 'repo' 
6. Click 'Generate token'
7. Copy the token

### Add remote

In Gitpod, in the menu (usually designed as 3 horizontal lines) choose `Terminal` and `New Terminal`. 

	cd wagtail
	git remote add USERNAME https://USERNAME:TOKEN@github.com/USERNAME/wagtail.git

### Create a branch and commit your work

	git checkout -b BRANCH_NAME
	git add PATH/TO/FILE.EXT
	git commit -m "MESSAGE"

### Submit a pull request

	git push USERNAME
    # remote: Create a pull request for 'BRANCH_NAME' on GitHub by visiting:
    # remote: https://github.com/USERNAME/wagtail/pull/new/BRANCH_NAME

Open the link and follow the instructions.

## Stop and continue

The Gitpod workspace will stop after 30 minutes of inactivity.
If your workspace has stopped, reload the browser or go to [your workspaces](https://gitpod.io/workspaces) and restart the workspace.
Gitpod automatically removes workspaces that are inactive for 14 days.
