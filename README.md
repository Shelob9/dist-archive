runcommand/dist-archive
=======================

Create a distribution .zip or .tar.gz based on a plugin or theme's .distignore file.

[![runcommand open source](https://runcommand.io/wp-content/themes/runcommand-theme/bin/shields/runcommand-open-source.svg)](https://runcommand.io/pricing/) [![CircleCI](https://circleci.com/gh/runcommand/dist-archive/tree/master.svg?style=svg)](https://circleci.com/gh/runcommand/dist-archive/tree/master)

Quick links: [Using](#using) | [Installing](#installing) | [Support](#support)

## Using

~~~
wp dist-archive <path> [<target>] [--format=<format>]
~~~

For a plugin in a directory 'wp-content/plugins/hello-world', this command
creates a distribution archive 'wp-content/plugins/hello-world.zip'.

You can specify files or directories you'd like to exclude from the archive
with a .distignore file in your project repository:

```
.distignore
.editorconfig
.git
.gitignore
.travis.yml
circle.yml
```

Use one distibution archive command for many projects, instead of a bash
script in each project.

**OPTIONS**

	<path>
		Path to the project that includes a .distignore file.

	[<target>]
		Path and file name for the distribution archive. Defaults to project directory name plus version, if discoverable.

	[--format=<format>]
		Choose the format for the archive.
		---
		default: zip
		options:
		  - zip
		  - targz
		---

## Installing

Installing this package requires WP-CLI v0.23.0 or greater. Update to the latest stable release with `wp cli update`.

Once you've done so, you can install this package with `wp package install runcommand/dist-archive`.

## Support

This WP-CLI package is free for anyone to use. Support, including usage questions and feature requests, is available to [paying runcommand customers](https://runcommand.io/pricing/).

Think you’ve found a bug? Before you create a new issue, you should [search existing issues](https://github.com/runcommand/sparks/issues?q=label%3Abug%20) to see if there’s an existing resolution to it, or if it’s already been fixed in a newer version. Once you’ve done a bit of searching and discovered there isn’t an open or fixed issue for your bug, please [create a new issue](https://github.com/runcommand/sparks/issues/new) with description of what you were doing, what you saw, and what you expected to see.

Want to contribute a new feature? Please first [open a new issue](https://github.com/runcommand/sparks/issues/new) to discuss whether the feature is a good fit for the project. Once you've decided to work on a pull request, please include [functional tests](https://wp-cli.org/docs/pull-requests/#functional-tests) and follow the [WordPress Coding Standards](http://make.wordpress.org/core/handbook/coding-standards/).

runcommand customers can also email [support@runcommand.io](mailto:support@runcommand.io) for private support.


