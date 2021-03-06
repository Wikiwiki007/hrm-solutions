[![Build Status](https://travis-ci.org/atesgoral/hrm-solutions.svg?branch=master)](https://travis-ci.org/atesgoral/hrm-solutions)

# Human Resource Machine solutions

This repo contains working solutions, in hopes of exchanging ideas to collaboratively come up with the most/size.speed optimized solutions (or simply to help those out there who are stuck). Even though the programs are created through a drag-and-drop interface within the game, copy/paste from/to the clipboard works as assembly source code seen in this repo.

[Top Scores and more info.](http://atesgoral.github.io/hrm-solutions/)

## File Naming Convention

The file naming convention used is:

Inside a folder called `<level>-<level name>-<size par>.<speed par>`, `[size].[speed].asm`

Where `size` and `speed` are the number of commands and steps of the solution, which is deemed by the game as size and speed optimized if they are equal to or less than the par numbers in its folder's name.

For example, `07-Zero-Exterminator-4.23/4.23.asm` means the solution is both size and speed optimized.

## Contributing

Please issue a pull request while keeping in mind:
* The file naming convention is met
* If you're a new contributor, edit the contributors.yml file to add yourself
* Make sure your new solution passes tests (see below)

## Testing

You need Node.js 4.1+ to be installed.

`npm install` to get all dependencies

`npm test` to run tests.

## Tools Used

The tests involve the static/runtime analysis and benchmarking of each solution by utilizing:

* [hrm-parser](https://github.com/nrkn/hrm-parser) by [@nrkn](https://github.com/nrkn) for static analysis of programs
* [hrm-cpu](https://github.com/nrkn/hrm-cpu) by [@nrkn](https://github.com/nrkn) for running programs and runtime analytics
* [hrm-level-data](https://github.com/atesgoral/hrm-level-data) by [@atesgoral](https://github.com/atesgoral) for level metadata for providing level constraints
* [hrm-level-inbox-generator](https://github.com/atesgoral/hrm-level-inbox-generator) by [@atesgoral](https://github.com/atesgoral) for randomly generating level-appropriate inboxes for benchmarking
* [hrm-level-outbox-generator](https://github.com/atesgoral/hrm-level-outbox-generator) by [@atesgoral](https://github.com/atesgoral) for determining the expected outboxes for given level + inbox for benchmarking
