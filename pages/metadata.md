---
permalink: /metadata/
title: Metadata, explained
---

Every blog post requires a bit of metadata called front matter. This is
where the post's title, authors, tags, banner image, excerpt, and
description live. It’s written in a format called YAML, a standard for
writing data computers can read that is also human readable. [It’s a
backronym meaning “YAML Ain’t Markup
Language.”](https://en.wikipedia.org/wiki/YAML)

Here are the required fields:

-   Title
-   Authors
-   Tags
-   Excerpt
-   Description

There are also a few optional fields:

-   Date
-   Image

Here is what each required field means and some guidelines for filling
them out:

Title
-----

The plain-text title of your post, surrounded by quotation marks. This
will be displayed prominently above the post, will show up in browser
tabs, and will be included in "share text" when the link appears on
Twitter, Facebook, and other social media platforms.

Titles should follow [sentence
case](https://pages.18f.gov/content-guide/capitalization/) (only the
first word should be capitalized), and they should tell the reader the
most important piece of information in the story. If you're launching a
product, communicate that in the title instead of something less
specific like *Continuing 18F’s commitment to open data.* If the title
of your product is descriptive of its function (for example, College
Scorecard) then it’s good to include it in the title. If it’s less clear
(for example, Midas) then it’s better to explain what the product does
and save the name for the first paragraph.

Authors
-------

A list of handles of teammates involved in authoring the post. They must
all be lowercase, and must match a name that appears in
[_data/authors.yml](https://github.com/18F/18f.gsa.gov/blob/staging/_data/authors.yml).
If your author doesn’t exist, [add it to the
file](https://github.com/18F/18f.gsa.gov/edit/staging/_data/authors.yml).
Names listed here will automatically be added to the post’s byline. In
addition, if the author has a bio on 18f.gsa.gov, posts tagged with
their name will automatically link to their bio. See our [authorship
section]({{
site.baseurl }}/content-guidelines/) for more information on how to choose authors.

Tags
----

A list of tags to associate with the post. These will appear, linked,
next to the post and will take readers to other posts that have this
tag. Sentences (for example, "how we work") are fine — there's no need to jam
phrases into one word. Follow our [tagging
guide]({{
site.baseurl }}/tagging/)
when choosing tags.

Excerpt
-------

A short plain-text snippet of the post to use as the "[nut
graf](https://en.wikipedia.org/wiki/Nut_graph)" that appears on the
home page. This should be the most important part of your post. Think of
it as what you would tell a friend if they asked you about your post. A
good excerpt is usually no more than two sentences long. No Markdown
allowed.

Description
-----------

A short, plain-text description of your post, surrounded with quotation
marks. No Markdown or HTML allowed. This can be the same as the excerpt
or it can be a sentence or two that you feel represents your post well.
It may appear next to your post on social media and other places that
fetch article metadata.

And here are the optional fields:

Image
-----

The main image of your post. A relative link, with a leading /. This
will appear in social media platforms when the post is shared. It can be
a different image than those that appear embedded in your post. Though
this section is optional, we highly encourage you to include a relevant
picture. It will increase the likelihood of your post being shared on
social media and can help give readers more information. Authors do not have to fill in the image path. You can simply insert your image into your Google Doc draft and a member of the blog team will fill it in during publishing. Full-width images should be 1600px wide. If omitted, a
standard image is used.

Date
-----

Overrides the default date set by Jekyll. When you create a post, you
give it a filename with a date in it. For example:
2015-10-01-post-title.md will automatically use October 1 2015 for the
date and /2015/10/01/post-title/ for the URL. If you don’t want the
publish date to match the filename, you can set this with a date string
in the form of YYYY-MM-DD. For example, date: 2015-01-01 would set the
date to January 1 2015. Published posts with a date in the future will
not appear on the site. Posts published on the same day will be listed
in chronological order instead of by most recent. To have posts listed
with the most recent appearing first, you can add a timestamp to the
front matter in the form YYYY-MM-DD HH:MM using 24-hour time.

Example front matter
--------------------
```
---
title: "New Federalist platform lets agencies quickly launch websites"
date: 2015-09-15
authors:
- melody
tags:
- our projects
- platform
- proactive federal partner
excerpt: "18F’s new Federalist platform is a suite of tools designed to
make it faster for government agencies to build websites that are
secure, responsive, and accessible."
description: "18F’s new Federalist platform is a suite of tools designed
to make it faster for government agencies to build websites that are
secure, responsive, and accessible."
image: /assets/blog/federalist/sbst-screenshot.jpg
---
```

Here’s a template you can paste directly into your draft:

```
---
title: ""
date: YYYY-MM-DD (optional)
authors:
-
tags:
-
-
-
excerpt: ""
description: ""
image: /assets/blog/slug/image.jpg/png/gif
---
```

Testing
-------

Every time we publish a blog post, [GitHub runs a suite of tests](https://18f.gsa.gov/2015/12/11/how-we-test-18f-gsa-gov/) that
check that the front matter for each post is correct. Right now,
“correct” means each of the required fields described above is filled
in. In the future, we also hope to have automated tests that check
whether the fields are formatted correctly. (If you currently list an
incomplete date for `date`, the test will pass, though in the future
it might fail.) We cannot publish the site if this test fails.
