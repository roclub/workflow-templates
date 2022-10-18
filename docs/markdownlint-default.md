# markdownlint-default
## Motivation
Without setting any specified rules, all markdownlint rules are applied for this workflow.
However, by linting a README sample of the most starred GitHub repositories, we found out that some specific markdown rules are violated in most of the cases although the repositories used state-of-the-art markdown style guides. Therefore, some rules of the markdownlint workflow have to be released since they are too strict and forbid quite useful style guides.

## Description
Rescaling length of lines, headings, code blocks etc .
```json
    "MD013": {
        "line_length": 400,
        "heading_line_length": 100,
        "code_block_line_length": 100,
        "code_blocks": true,
        "tables": true,
        "headings": true,
        "headers": true,
        "strict": false,
        "stern": false
      },
```
Enable to display shell commands without showing the output.
```json
    "MD014": false,
```
Enable inline HTML.
```json
    "MD033": false,
```
Code blocks do not necessarily need a specified language.
```json
    "MD040": false
```