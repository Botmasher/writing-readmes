# Writing READMEs

## 1. Welcome
- instructor: Walter
- compared to other things been doing with code docs seem stale
- it's not stale!
- cook up own READMEs
	- what documentation is
	- why it's important
	- incorporate into future projects
- this course is for you if:
	1. you write code
	2. you work with people who write code
- focus on the concepts not the code we'll document in this course

## 2. What Is Documentation?
- imagine a cookbook
	- documents what it takes to make delicious meals
	- might have all ingredients but it tells you how to put them together
- similar with code since documentation helps us understand other people's code
- instructor writes docs for all projects including [this course](https://github.com/udacity/ud777-writing-readmes)

## 3. Quiz: Who Is Documentation For?
- technical documentation often "written in plain English"
- written for humans
- written to make sense of code
- for OSS it's important since it helps gain users and contributors
- good documentation: people may want to use the code in their projects
- great documentation: people may want to contribute to your lib
- consider yourself, your coworkers, your users when you write

## 4. How Does Nijia Consume Documentation?
- use it to understand third-party libs and tools
- to get started running by looking for examples
- sad if documentation unavailable
	- not use lib
	- switch to lib with better doc
- how to figure out code when doc missing
	- dig through source code
	- examine with debugger
	- more advanced troubleshooting tools
	- it's "like reverse engineering somebody else's thought process"

## 5. Why Should Art Have Documented His Code?
- put a placeholder number and forgot to add to the README this was just a placeholder
- somebody called the number
- take a look at your older projects: what were you thinking?

## 6. Quiz: Introduction to READMEs
- sometimes docs can be overkill, like a cookbook for a single recipe
- README file is great for small projects
	- since the punchcard days
	- info about other files in the dir
	- usually in all caps to stand out
- check out these three READMEs:
	- What info do the above files have?
	- How is this info structured?
	- Are there patterns across the files?
	1. https://github.com/thoughtbot/factory_bot
		- many headers
		- clearly defined
		- links
		- how to get started
		- how to contribute
		- at bottom, licensing info and links
	2. https://github.com/zkat/can.viewify
		- by instructor's friend
		- shorter but still clear sections
		- installation
		- description
		- usage examples
		- section with an issue in the code
		- licensing
	3. https://github.com/udacity/create-your-own-adventure
		- from Udacity's Git and GitHub course
		- not much info
		- but lots of details on how to contribute
		- licensing
	- all three contain "the essential information" to get things up and running

## 7. Anatomy of a README
- Ledbetter is a project maintained by GitHub
- this README ought to "provide just enough context to get a user up and running with your code"
	- written for other humans
- title and description
	- capture project clearly and concisely
	- include logo if wanted
- must-knows about the code
	- installation instructions
	- dependencies
	- usage (how to run)
	- length of these depends on project
- don't make assumptions about end users
- "essential information" to write steps for getting started
	1. what are the exact steps to take to get this up and running?
	2. what must user already have installed/configured?
	3. what might be hard for user to understand about this right away?
- include example code to "show your end users proper usage of your code"
- taking on your own assumptions
	- you already know your code
	- but what about someone who's never seen it before?
	- do you assume that someone knows what recursion is or not?
	- in the end it's up to you how detailed to go

## 8. Quiz: Documenting a Growing Codebase
- reevaluate as you grow
- here are some common sections to evaluate
	1. copyright/licensing
		- "safer to be explicit"
		- include full text or link to it
		- [choosealicense](https://choosealicense.com/) helps distinguish between licenses based on your goals
	2. contributing
		- spell out your preferred ways
		- guidelines
		- code of conduct
	3. services that provide "shields"
		- code status shields for tests passing
		- third-party info for users giving helpful info about code
		- useful if "you're writing lots of tests in your code"
- do NOT overcomplicate things though
- other sections to consider:
	- known bugs
	- FAQs
	- table of contents
- sections to avoid including:
	- press coverage of your project
		- doesn't help us use your code
		- better for personal or project website
	- pics of your cat

## 9. Readable READMEs with Markdown
- possible to use any format including made-up ones
- but Markdown is useful and translatable to HTML
- MD is easy to skim
- write them more like recipes than unformatted blocks of text

## 10. Basic Markdown Syntax
- dialects include "GitHub Flavored Markdown"
- `**bold**`, `*italics*`, `_italics_`, `code`, `# h1`, `## h2`, `### h3`
- markdown: https://help.github.com/articles/getting-started-with-writing-and-formatting-on-github/
- GitHub-flavored differences: https://help.github.com/categories/writing-on-github/

## 11. Quiz: Basic Markdown Syntax
- Question: write the markdown for the following:
	- the words "Here is your task" marked as header level 1
	- the word "code" marked as code
	- the word "here" marked as bold
	- the word "there" marked as italicized

## 12. More Markdown Syntax
- explore even more: https://help.github.com/articles/getting-started-with-writing-and-formatting-on-github/
- lists
	- ordered lists
	- unordered lists
- links
- large code blocks
- fall back to HTML whenever you need to
- save with an `.md` extension
- to preview use https://dillinger.io/ or a Sublime plugin https://packagecontrol.io/packages/GitHub%20Flavored%20Markdown%20Preview

## 13. Markdown Syntax Practice
- useful for READMEs because requires less code than writing them in HTML
- try converting some HTML into Markdown:
```
<h1>My Fabulous Recipe</h1>

<p>This recipe for <strong>cereal and milk</strong> has been passed down my family for months.</p>

<h2>Ingredients</h2>

<ul>
	<li>Cereal (you can find cool cereals <a href="www.example.com/coolcereals">here</a>)</li>
	<li>Milk</li>
</ul>

<h2>Directions</h2>

<p>If I were writing these out as <em>code</em>, it might look something like this:</p>

<pre><code>if bowl is empty:
	add cereal
if bowl only has cereal in it:
	add milk
</code></pre>
</body>
```
- Answer:
```
# My Fabulous Recipe

This recipe for **cereal and milk** has been passed down my family for months.

## Ingredients

* Cereal (you can find cool cereals [here](www.example.com/coolcereals))
* Milk

## Directions

If I were writing these out as _code_, it might look something like this:
```
```
if bowl is empty:
	add cereal
if bowl only has cereal in it:
	add milk
```

## 14. Document Everything!
- now you can write basic documentation
- explore other kinds of documentation
- it's not just about code working
	- make it easy to use
	- make it easy to maintain
- documented code is meant for humans
- challenge: write a README for some of your old projects
- make documentation a priority!
