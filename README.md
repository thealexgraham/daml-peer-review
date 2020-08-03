# daml-peer-review

A DAML proof of concept that models a peer reviewed journal

## workflow
```
author    : create Paper
author    : request publication from journal
journal   : create Review with paper, required votes and reviewers
reviewers : approve, disapprove
journal   : resolve review
    based on number of votes, and requirements, can either
        Publish : adds paper to list of papers
        Deny    : send paper back to author
```
