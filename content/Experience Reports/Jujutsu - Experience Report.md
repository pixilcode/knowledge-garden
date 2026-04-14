---
title: Jujutsu - Experience Report
tags:
  - experience-report
  - blog-post-draft
  - topic-git
  - tool
  - topic-software-development
date: 2026-04-14
---

[Jujutsu on Github](https://github.com/jj-vcs/jj)

Jujutsu (or `jj` for short) is a distributed version control system that is works with _changes_ instead of _commits_. A _change_ is a collection of edits that can be modified, as opposed to a commit which is a fixed collection of edits.

## Liked
- Thinking in terms of changes rather than commits allowed me to organize my changes a lot easier and more coherently
- Any time I realize that I forgot to do something in a previous commit, I could just `jj edit <changeID>`, make my change, then go back to the commit that I was working on
- Organizing a bunch of changes that I've just made into individual commits is easy, even if I forgot to commit as I went. For each change:
    - `jj new -B @ -m "description of specific change" --no-edit`
    - `jj squash -i` (or `jj squash src/main.rs` if a file only has edits relating to one specific change
- `jj undo` is _so useful_ for undoing mistakes that you made, and it's so easy to use!
- `jj` is completely compatible with `git`. None of my coworkers even know that I'm using it, so I don't have to try and convince them to learn a new VCS (although I might now that I know how _awesome_ it is!)

## Disliked
- Working with Github branches was not easy on the first go. I had to manually update the branches that I was working on using `git`, which was not ideal
    - I haven't looked very much into how `jj` works with Git branches, so there may be an easier way

## Overall Impression

I **love** `jj`! I think that it's going to be my VCS for the next little bit. I'm impressed with all of the improvements that they've made to `git`. I also like that I can use it with any project that uses `git` without having to do a thing.

In conclusion, `jj` matches my dream workflow so well. 10/10 would recommend `jj`.