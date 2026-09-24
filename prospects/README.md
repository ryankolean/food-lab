# Prospects

Recipes and ideas found elsewhere that haven't been made yet. Everything here gets reviewed, logged, and
then either stubbed into a Food Lab section or skipped.

| Source | Log | How to add to it |
| --- | --- | --- |
| Instagram Reels, posts and saved collections | [`instagram.md`](instagram.md) | `/ig-intake <url>` in Claude Code |

## Running the Instagram intake

On your own computer, in a clone of this repo:

```bash
claude --chrome
```

Make sure you're logged in to Instagram in that Chrome, then run:

```
/ig-intake https://www.instagram.com/<you>/saved/food/<collection-id>/
/ig-intake https://www.instagram.com/reel/<shortcode>/
```

You can pass several URLs at once. The skill:

1. skips posts already in the log
2. opens each new post in Chrome, reads the caption, pinned comment and on-screen text, and screenshots
   frames through the video (it can't hear audio)
3. logs each post with what it found
4. asks which posts to stub
5. opens one PR with the log update and the new stubs

It never likes, follows, comments on or unsaves anything, and it never asks for your password.
