# Git & GitHub workflow

This document is the best practice guide that contains the rules to workflow while contributing to LocalStack projects using Git & GitHub.

## Prerequisites

The basic prerequisites are:

- [GitHub Account](https://github.com/home)
- [Git CLI](https://git-scm.com/)

We also recommend you to authenticate [Git with GitHub using SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh).

## Fork and clone

In your browser, visit: https://github.com/localstack. Find the project that you would like to contribute to and open the appropriate link. In the upper left corner, you will find an option to fork the project. Please click on it to create a fork/copy of the repository on your profile.

- On your terminal, clone the repository by running the command where  `your-username`  represents your GitHub username while the  `project-slug`  signifies the name of the project you are cloning.

	```sh
	git clone https://github.com/<your-username>/<project-slug>/
	```
- Enter into the newly created directory by running the following command on your terminal:

	```sh
	cd <project-slug>
	```
- Configure the upstream for your fork so that  `git`  can sync work from the upstream, by running the following command:

	```sh
	git remote add upstream <link_of_original_repository>
	```
- Check if upstream is configured by running the command:

	```sh
	git remote -v
	```

## Making a contribution

After you set up your fork, start contributing code, docs and fixes.

- Create a branch on your local machine: 

	```sh
	git checkout <branch-name>
	```
- Commit the changes:

	```sh
	git add <file> <file> ...
	git commit -m "relevant commit message"
	```
- Push the changes to the remote forked repository.

	```sh
	git push -u origin <branch-name>
	```

You can now create a pull request to get your changes merged into the upstream branch of the specific repository. 
