---
permalink: /publishing-process/
title: How to get your blog post published
---

First, it might be a good idea to check out our [mission brief]({{
site.baseurl }}/mission-brief/), if you haven't already.

At 18F we keep a [private GitHub
repo](https://github.com/18f/blog-drafts) for proposing ideas,
discussing drafts, and managing the editing and approval process.

We use five milestones to manage blog post issues.

1. `idea`
1. `draft`
1. `to edit`
1. `ready to approve`
1. `approved`

In this section, we'll walk you through each of the milestones.

## Idea: How do I create a new post?

Every blog post begins as an issue with the `idea` milestone. You should feel free to file `idea` issues even if you don't have a draft or don't think you can write the post. Any team member can "pick up" issues with the `idea` tag and begin
drafting a post. Issues are picked up when someone assigns themselves to the issue.

To create an issue in the blog-drafts repo, you can [click here to have a preformatted issue created for you](https://goo.gl/pt0alV), or you can manually create a new issue and copy the code below into the issue description. 

```
## Audience

As a [type of audience], I want [to read or learn something], so
that [some benefit is had].

## Goal of blog post

## Description

## Imagery ideas

## Who needs to clear the post

- [ ] @18f/blog
- [ ] Gia - GSA Congressional Affairs (OCIA)
- [ ] Cat - GSA Office of Communications and Marketing (OCM)
```

The people in the "who needs to clear this post" section above are required for every blog post, but you should also include anybody inside or outside of our team who should have eyes
on your post. This may include

- An agency partner
- Expert reviewer
- 18F project lead
- 18F guild

**Blog posts without all of the above information will be marked with
the `incomplete` label until they are fully filled in. We are happy to
talk through the idea but will not review a draft of a post with the
`incomplete` label.**

If you’re unsure of what to put in any section, drop in on a blog huddle
or hit us up on Slack (#blog).

### Who are these people that need to approve my blog post?

#### Inside 18F

To approve your blog post, the 18F comms team is looking for 18F style,
general connection to 18F and GSA’s mission, and a complete structure
with a beginning, middle, and end. The team is also on the lookout for
additional reviewers that might be required for certain posts (for
example, legal, contracting officers, senior management, compliance experts).

#### Inside GSA

Gianelle (Gia) Rivera is the Technology and Digital Services Policy Advisor at
GSA’s Office of Congressional and Intergovernmental Affairs (OCIA). OCIA
“serves as advisor to the Administrator and GSA leadership and
supervises and maintains agency liaison with all members of Congress and
congressional committees. The office also serves as liaison with state
and local Government officials and their official national
organizations.” Gia reads our blog posts with the eye of a Member of
Congress or congressional staffer and makes sure our posts align with
wider GSA communications and messages.

Cat Langel is a public affiars officer in the Chicago (Region 5) Office of Communications and Marketing (OCM). She is responsible for reviewing posts for GSA’s blog and 18F. Cat is our primary contact in OCM. She reviews posts and then will flag posts that require approval from other people in OCM or other GSA offices. Cat is looking for messaging concerns in blog posts and to coordinate our efforts with the other technology offices across GSA.

## Draft: What steps should I take when drafting my post?

1. Once an issue is in writing mode, move it to the `drafts`
milestone.
2. Create a Google Doc in [the Blog
folder](https://drive.google.com/a/gsa.gov/#folders/0B-y3CqI2T1nndGE0c191NGtUTEU)
with the text of your post.
3. Copy the code below and add it to the top of your draft. (Find more information about these fields in the [metadata section](https://pages.18f.gov/blogging-guide/metadata/).)

```
GitHub issue URL:
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



Go back to the issue in blog-drafts, edit the issue description, and paste in a link to your draft.

## To edit: How do I get my post edited?

Once the post is drafted and ready to be edited by the blog team:

1. Move it to the `to edit` milestone.
1. A member of the blog team will edit the post and work with you to
resolve any issues.
1. After you've resolved any edits with the blog team, send the draft to any outside agency or other 18F team who needs to review the post.

## Ready to approve: How do I get my post approved?

When a post has been cleared by the blog team and any outside
reviewers, a blog team member will take responsibility for getting the post approved and published. They will:

- Move it to the `ready to approve` milestone
- Tag Cat and Gia in the Google Doc draft for approval.
- Add the labels `for review -ocia` and `for review- ocm`.

Cat and Gia need to actively approve the post before it can be published. As each person approves the post, a member of the blog team with remove the appropriate `for review` label and will check the boxes in the issue description. Our Infrastructure Director, Noah Kunin, must approve any communications regarding cloud.gov, an Authority to Operate (ATO), or security in general.

If your post is announcing an 18F project that collaborates with an
outside agency, or if you're providing an update or more information on
an existing 18F project, you must complete a [Comms
Plan](https://docs.google.com/document/d/1GgaL-qJv_gpZPsnkvCsRyAdwUDQCxXo0zIRTPVnr9xQ/edit).
This is a document to be given to the communications office,
congressional affairs office, and senior management at GSA. A
blog team member will help you complete this document.

After the above-mentioned folks have made comments and suggestions,
and after you’ve resolved them, a blog team member will move the issue to the `approved`
milestone. The blog team will work with you to schedule when the post will be published and will add the post to the 18F Editorial Calendar.

## Approved: How do I get my blog post published?

When the post is ready to be published, a member of the blog team will:

  1. Convert the post to markdown.
  1. Open a pull request to post it to the staging branch of 18f.gsa.gov for final review. Any final edits will be
discussed in #blog.
  1. After all edits are discussed and the author has approved the final post, ping @gregboone or @elainekamlley to rebuild the site and publish the post. 
  1. Once the post goes live, post the live URL in a
comment and close the issue.
