## BugMagnet AI Assistant

AI assistant command for comprehensive test coverage and bug discovery. Use it for:

- Writing characterisation tests (documenting existing behaviour to make future changes easier)
- Test coverage and gap analysis
- Undocumented/unclear behaviour and state transition analysis
- Exploratory testing and advanced coverage analysis
- Applying common testing heuristics to detect bugs and feature gaps

The command contains extensive test heuristics and information on common coding mistakes from [BugMagnet](https://www.bugmagnet.org) and [Humans vs Computers](https://gojko.net/books/humans-vs-computers/).

## Installation

For Claude Code, copy <commands/bugmagnet.md> into your command directory (usually `.claude/commands`).

## Usage

For Claude Code, run the slash command and point it to a file you want to analyze. For example:

```
/bugmagnet src/auth/cognito-auth-session.js
```

## Compatibility

The BugMagnet command is primarily developed for and tested with Claude Code.
However, there is nothing specific about Claude Code in it, and in theory it
should be compatible with other AI coding assistant tools.

The command is generic enough to be used with any programming language and
testing tool that the AI assistant knows about, and generally follows existing
project guidelines for tooling and tests.

## Customization

The command will check CONTRIBUTING.md, CONTRIBUTING.txt, README.md or
README.txt files in the main project directory for additional instructions
related to test writing or heuristics, so you can add additional cases or
customization there.

The command will specifically ask you for additional documents or guidelines
at the end of phase 1, so you can provide information to customize the execution 
in that step as well.


## LICENSE

MIT, see <LICENSE.md>

