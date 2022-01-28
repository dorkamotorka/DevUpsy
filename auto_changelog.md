# Changelog

Changelog is basically a file that stores/documents added features, changes, bugfixes etc. of your source code repository.
It combines code commits into meaningful log including the timestamp, therefore giving a high overview of that changes that took place.

Managing changelog can be automated, but in most cases the user should conform with the standard structure of the commits in order to do so.

There is lots of available changelog generators. Consider some options here: https://www.freecodecamp.org/news/a-beginners-guide-to-git-what-is-a-changelog-and-how-to-generate-it/

I'm personally using **generate-changelog** and it can be installed using:

	npm install generate-changelog -g 

If you projects root consist of a valid **package.json** file, than you can invoke:

	changelog generate

which generates a CHANGELOG.md file. It's good practice to run that locally, since you might have to edit some commites or remove them from the changelog list.

Note that before running I had conventional commits setup using **commitlint** and **Husky**.

## Integration with GitHub Actions

You can also add it to your GitHub Actions pipeline, automating it on events of your preference.
I have added a simple example to this repository under **.github/workflows/.release.yaml**. 
Note that this action needs to be manually dispatched.
