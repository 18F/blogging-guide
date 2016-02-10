---
title: Tagging
---

Tags allow us to organize our blog posts, and they provide readers with
an easy way to explore a particular topic. They're also useful for
sending a collection of posts to someone with a single link. To keep
tags useful, we aim to include in the tag list only necessary tags and
to apply only a handful of tags (3-5) to any single post.

If you’re writing the first post about a long-term delivery project,
please create a new project specific tag. For example, `betafec`,
`uscis`, or `calc`. Beyond organizing posts about your project,
these tags will also be used to help pull relevant blog posts into other
parts of 18f.gsa.gov. If you have questions about what to call your
project, or if the project name changes, drop into #blog to discuss it
with the team.

Consulting projects should be tagged with the type of service. For
example, `rfp ghostwriting`, `discovery`, or `protosketching`.

Please check the list of existing tags before adding tags to your post.
If you’d like to create a new tag for your post, it should be one that
is likely to be reused. If you’ve reviewed the list of existing tags and
would still like to create a new one, please keep the following criteria
in mind:

-   **Applicability**: Is the tag likely to apply to other blog posts, or is it relevant only to your post? It’s better to have one tag that covers a couple areas than a number of ultra-specific tags. For example, use `agile` instead of also adding `agile development`, `agile techniques`, and `agile methodologies`.
-   **Time sensitivity**: Will this tag continue to be useful in the future (short- and longer-term), or is it useful only within a limited timeframe?
-   **Overlap**: Is your proposed tag different enough from existing tags to warrant being created? Before creating a new tag, review the full tag list to see if there’s another similar tag you can use instead.

### Formatting

When typing tags or creating new ones, please follow these guidelines.

- Use all lowercase for tag names, even for proper nouns and acronyms
(i.e. "18F" should be "18f", "GSA" should be "gsa"). We format them when
we generate the site.
- **Separate words with spaces** not dashes or underscores
(**Correct:** "the hub", **Incorrect:** "the-hub" or "the_hub")
- Numbers are allowed
- List tags like this in the frontmatter of posts:

```yaml
tags:
- 18f
- how we work
- tagging
```

If you add a new tag to this list, it will be created and used with your
post.

### Why is this important?

If you generate the site locally and look in the `_site/tags/` folder
you might notice a few folders that look like they break these rules.
There are a few reasons for that.

When Jekyll generates the site, it makes a folder and an `index.html`
file inside it for each tag. When it does that it automatically
substitutes all spaces with `-`. This is why it's important to always
use spaces and not dashes. When Jekyll sees, for example, `how we
work` on one post, it generates the `how-we-work` folder in your
`_site/tags` directory. Then, if it sees `how-we-work` on a
different post it overwrites the `how-we-work` folder it already
created and you end up with an incomplete archive of only the posts
tagged `how-we-work`. The same is true for capitalization.

All this means we need to be consistent and the formatting rules above
are how we've decided to stay consistent.

### Redirections

When we first got the site started we used the same rules but didn't
rely on [Jekyll's way of generating tag
archives.](https://github.com/jekyll/jekyll-archives) We did it on our
own and https://18f.gsa.gov/tags/how%20we%20work was the archive for the
`how we work` tag. The catch was that
https://18f.gsa.gov/tags/how-we-work was _also_ a page that was an
archive for anything we didn't tag correctly. Other examples are
`tags/18F events` and `tags/18F Consulting` which had counterparts
at: `tags/18f events` and `tags/18f consulting`.

When we fixed that problem we also set up redirects for the older URLs
to go to the right place. That's why you see both `how we work` and
`how-we-work` folders in the `_site` directory. One (`how we
work`) is the redirect pointing to the other (`how-we-work`). We do
this to make sure people with bookmarks, other sites, and search engines
all get to the right place. To see how we do it, check out [this pull
request](https://github.com/18F/18f.gsa.gov/pull/921) which added the
redirects and the [`jekyll-redirect-from`
plugin](https://github.com/jekyll/jekyll-redirect-from) we use to make
it happen.

With that in mind, please, use [the list of current tags](https://18f.gsa.gov/tags/) and
the [formatting rules above](#formatting) as your guide for tagging
posts, _not_ the contents of your `_site/tags` folder.

### Which tags should I use?

Refer to [this list of current tags](https://18f.gsa.gov/tags/) to see which ones best fit your post.
