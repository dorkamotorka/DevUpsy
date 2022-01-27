# Conventional GitHub Commits

The far most easy and useful thing you can thing is create meaningful commits. 
If you are working alone or on a team you want to standardize they way code changes are logged. You will be grateful once, you have to backtrack a bug or an issue.
Similarly this applies to automated tools that tend not to work if your commits don't follow a specific structure.

The following guide provides a nice reference to set things using Git: [commitlint.js.org](https://commitlint.js.org/#/guides-local-setup?id=install-commitlint)

If you prefer to just get through it fast, copy-paste and run the following commands:

	npm install --save-dev @commitlint/{cli,config-conventional}
	echo "module.exports = { extends: ['@commitlint/config-conventional'] };" > commitlint.config.js
	npm install husky --save-dev
	npx husky install
	npx husky add .husky/commit-msg 'npx --no -- commitlint --edit $1'
# or
