---
permalink: /publishing-process/
title: How to get your blog post published
---

First, it might be a good idea to check out our [mission brief]({{
site.baseurl }}/mission-brief/), if you haven't already.

At 18F,  we use a combination of a [private GitHub
repo](https://github.com/18f/blog-drafts), a [private kanban board](https://github.com/18F/blog-drafts/projects/1), and an [editorial calendar](https://calendar.google.com/calendar/embed?src=gsa.gov_pkkbf53u1m6is9gi76v1l8i5j8%40group.calendar.google.com&ctz=America/New_York) to manage the blog editing and approval process. Blog posts are drafted in Google Docs, editing is managed in GitHub, the process is tracked with the kanban board, and posts are scheduled on the calendar. We discuss all of this in the #blog Slack channel.

We use six milestones on GitHub to manage blog post issues.

1. Idea
1. Coach
1. Author writing
1. To edit
1. Ready to schedule
1. Scheduled

In this section, we'll walk you through each of the milestones.

## Idea: How do I create a new post?

Every blog post begins as an issue with the “idea” milestone. You should feel free to file “idea” issues even if you don't have a draft or are unsure if your idea is headed in the right direction. Head over to #blog or #outreach if you'd like talking through your ideas.

When you [create a new issue](https://github.com/18F/blog-drafts/issues/new), the following template will auto-fill.

```
## Audience

As a [type of audience], I want [to read or learn something], so
that [some benefit is had].

## Goal of blog post

## Outline

## Imagery ideas

## Who needs to clear the post

- [ ] @18f/blog
```

Include anybody inside or outside of our team who should have eyes
on your post. This may include

- An agency partner
- Expert reviewer
- 18F project lead
- 18F guild

**You should feel free to file issues for ideas that are in the early stages and may need some discussion before you can answer these questions, but in order for a post to move out of the idea milestone and into the process it must meet the following acceptance criteria:**

>A blog post must have a blog-drafts issue that describes the audience with a user story, identifies a single goal for the post, and includes a draft outline with a minimum of five items.

If you have any questions, talk to us on Slack in #blog.

### What's the approve process like?

#### Inside 18F

To approve your blog post, the 18F comms team is looking for 18F style,
general connection to 18F and GSA’s mission, and a complete structure
with a beginning, middle, and end. The team is also on the lookout for
additional reviewers that might be required for certain posts (for
example, legal, contracting officers, senior management, compliance experts).

#### Inside GSA

The 18F blog team shares blog posts with the Office of Strategic Communications (OSC) through a shared Google Calendar. OSC reviews blog posts for alignment with GSA messaging, legal, procurement, privacy, and other laws and regulations. 18F is responsible for language, style, and audience decisions, but we work with OSC to resolve any issues. OSC does not proactively need to approve a blog post for 18F to publish it.

## Coach: What steps should I take when drafting my post?

1. When you’re ready to take on a post, ping Andre Francisco to talk out the audience and broad goals of your post. This talk can be a short Slack conversation, an email back and forth, or a quick video chat, but it’s important to make sure the blog post is on the right track from the beginning so we don’t waste staff hours on posts that are unlikely to make it to publication.
2. When Andre has WIP limit space to coach the post, he will assign it to himself and work with you to set up a time to talk. Andre will talk you through the metadata you filled out in the idea milestone and make sure you’re on the path to success.

## Author writing: Where should I draft my post?

1. After you’ve talked to Andre, create a Google Doc in [the Blog
folder](https://drive.google.com/a/gsa.gov/#folders/0B-y3CqI2T1nndGE0c191NGtUTEU)
with the text of your post.
2. Copy the code below and add it to the top of your draft. (Find more information about these fields in the [metadata section](https://pages.18f.gov/blogging-guide/metadata/).)

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
image: /assets/blog/slug/image.jpg/png/gif
---
```

3. Go back to the issue in blog-drafts, edit the issue description, and paste in a link to your draft.
4. Change the milestone on the issue to “author writing.”

## To edit: How do I get my post edited?

Once the post is drafted and ready to be edited by the blog team:

1. Move it to the “to edit” milestone.
1. A member of the blog team will assign themselves the post when they have WIP limit space, edit the post, and work with you to resolve any issues.
1. After you've resolved any edits with the blog team, a member of the blog team will change the milestone to “ready to approve.”

## Ready to approve: How do I get my post approved?

When a post has been cleared by the blog team, the editor will work with you to determine if they are any outside stakeholders or other 18F teams that need to review the post. Once the post has cleared those people, a blog team member will take responsibility for getting the post scheduled and published. They will:

- Add the post to the editorial calendar
- Send the calendar item to OSC

If your post is announcing an 18F project that collaborates with an
outside agency, or if you're providing an update or more information on
an existing 18F project, you must complete a [Comms
Plan](https://docs.google.com/document/d/1GgaL-qJv_gpZPsnkvCsRyAdwUDQCxXo0zIRTPVnr9xQ/edit). This will help Outreach coordinate with OSC for any press outreach, social media post, and other promotion.

After the above-mentioned folks have made comments and suggestions,
and after you’ve resolved them, a blog team member will move the issue to the "scheduled"” milestone.

## Approved: How do I get my blog post published?

When the post is ready to be published, a member of the blog team will:

  1. Convert the post to markdown.
  1. Open a pull request and send you a Federalist preview of the blog post. They will ask you for final edits in #blog.
  1. After you have approved the final post, a member of the blog team will merge the pull request and your post will be live.
  1. Once the post goes live, a member of the blog team will tweet it out from the 18F account and post the live URL in a comment on the GitHub issue and close the issue.
