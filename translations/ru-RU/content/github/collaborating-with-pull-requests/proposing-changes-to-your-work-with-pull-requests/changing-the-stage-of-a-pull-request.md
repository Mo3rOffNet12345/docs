---
title: Changing the stage of a pull request
intro: 'You can mark a draft pull request as ready for review{% ifversion fpt or ghae or ghes or ghec %} or convert a pull request to a draft{% endif %}.'
permissions: People with write permissions to a repository and pull request authors can change the stage of a pull request.
product: '{% data reusables.gated-features.draft-prs %}'
redirect_from:
  - /github/collaborating-with-issues-and-pull-requests/proposing-changes-to-your-work-with-pull-requests/changing-the-stage-of-a-pull-request
  - /articles/changing-the-stage-of-a-pull-request
  - /github/collaborating-with-issues-and-pull-requests/changing-the-stage-of-a-pull-request
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Pull requests
shortTitle: Change the state
---

## Marking a pull request as ready for review

{% data reusables.pull_requests.mark-ready-review %}

{% ifversion fpt or ghae or ghes or ghec %}
{% tip %}

**Tip**: You can also mark a pull request as ready for review using the {% data variables.product.prodname_cli %}. For more information, see "[`gh pr ready`](https://cli.github.com/manual/gh_pr_ready)" in the {% data variables.product.prodname_cli %} documentation.

{% endtip %}
{% endif %}

{% data reusables.repositories.sidebar-pr %}
2. In the "Pull requests" list, click the pull request you'd like to mark as ready for review.
3. In the merge box, click **Ready for review**. ![Ready for review button](/assets/images/help/pull_requests/ready-for-review-button.png)

{% ifversion fpt or ghae or ghes or ghec %}

## Converting a pull request to a draft

You can convert a pull request to a draft at any time. For example, if you accidentally opened a pull request instead of a draft, or if you've received feedback on your pull request that needs to be addressed, you can convert the pull request to a draft to indicate further changes are needed. No one can merge the pull request until you mark the pull request as ready for review again. People who are already subscribed to notifications for the pull request will not be unsubscribed when you convert the pull request to a draft.

{% data reusables.repositories.sidebar-pr %}
2. In the "Pull requests" list, click the pull request you'd like to convert to a draft.
3. In the right sidebar, under "Reviewers," click **Convert to draft**. ![Convert to draft link](/assets/images/help/pull_requests/convert-to-draft-link.png)
4. Click **Convert to draft**. ![Convert to draft confirmation](/assets/images/help/pull_requests/convert-to-draft-dialog.png)

{% endif %}

## Дополнительная литература

- "[About pull requests](/github/collaborating-with-issues-and-pull-requests/about-pull-requests)"
