# Changelog

Changelog is basically a file that stores/documents added features, changes, bugfixes etc. of your source code repository.
It combines code commits into meaningful log including the timestamp, therefore giving a high overview of that changes that took place.

Managing changelog can be automated, but in most cases the user should conform with the standard structure of the commits in order to do so.

There is lots of available changelog generators. Consider some options here: https://www.freecodecamp.org/news/a-beginners-guide-to-git-what-is-a-changelog-and-how-to-generate-it/

I'm personally using **generate-changelog** and it can be installed using:

	npm install generate-changelog -g 

If you projects root consist of a valid **package.json** file, than you can invoke:

	changelog generate

which generates a CHANGELOG.md file.

Note that before running I had conventional commits setup using **commitlint** and **Husky**.
