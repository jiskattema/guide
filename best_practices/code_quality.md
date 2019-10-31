# Code Quality

There are several ways to improve software quality and find bugs quickly and easily.
By following a set of conventions, code will look 'cleaner' and be more understandable.
It will also help spot syntax errors and other errors early, without having to run or compile all the time.

## Coding style

A coding style gives guidance on those parts of programming that are irrelevant to the compiler or interpreter.
For instance, what do you call your variables? do you use spaces or tabs for indentation? Where do you put comments? etc.

Here is a very nice article about why coding styles matter, and increase software quality:
[Improving software quality, why Coding Style Matters](http://coding.smashingmagazine.com/2012/10/25/why-coding-style-matters/)

For style guides see the different languages in [the Language Guides](language_guides/languages_overview.md).
Google has a style guide for most languages [google style guide page](https://code.google.com/p/google-styleguide/).

## Editorconfig

Use [editorconfig](http://editorconfig.org/) to adhere to the basic code style rules.

Using editor config is not necessary, but saves a lot of time and keeps developers from straying
from the style of choice and helps to avoid some problems caused by formatting differences
(line ending, tabs vs spaces).

There is support for editorconfig in most editors.
The [Editorconfig website](http://editorconfig.org/) provides plugins for your editor of choice.
If you use eclipse, use [this plugin](https://github.com/ncjones/editorconfig-eclipse).

The eScience Center has a [shared editor config file](https://raw.githubusercontent.com/NLeSC/exemplum/master/.editorconfig)

## Automatic code formatters and linters

These are small programs that check if your code follows a specific coding style.
Some code formatters can find more issues (unused variables, missing documentation, ...)
They are often langauge dependent, and can be integrated with an editor.

## Online software quality improvement tools

There are several web services that analyze code and make the quality of the code visible.

Code quality analysis services are web applications which have the following features:

 * Automaticly analyse your code after a Github push
 * Usually free for open source projects
 * Most supports multiple programming languages, but not every language will have the same level of features
 * Grade or score for the quality of all of the code in the repository
 * List of issues with the code, grouped by severity
 * Drill down to location of issue
 * Default list of checks which the service provider finds the best practice
 * Can be configured to make the list of checks more strict or relaxed
 * Can be configured to ignore files or extensions
 * Can read configuration file from repository
 * Tracks issues over time and send alerts when quality deteriorates
 * Optionally reports on code coverage generated by a CI build

See the [language guides](language_guides/languages_overview.md) for good options per language.

For a list of choices see http://shields.io/ or https://github.com/ripienaar/free-for-dev#code-quality

## Name spaces

If your language supports namespaces, use **nl.esciencecenter**

## Code reviews

See the [Code Reviews](./code_review.html) section.