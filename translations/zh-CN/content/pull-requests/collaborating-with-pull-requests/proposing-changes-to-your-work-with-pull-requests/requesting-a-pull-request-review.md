---
title: 请求拉取请求审查
intro: 创建拉取请求后，您可以请求特定人员审查您提议的更改。 如果您是组织成员，还可以请求特定团队审查您的更改。
product: '{% data reusables.gated-features.multiple-pr-reviewers %}'
redirect_from:
  - /github/collaborating-with-issues-and-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review
  - /articles/requesting-a-pull-request-review
  - /github/collaborating-with-issues-and-pull-requests/requesting-a-pull-request-review
  - /github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Pull requests
shortTitle: 请求 PR 审查
---

存储库属于个人帐户（单一个人所有者）或组织帐户（与众多协作者或维护者的共享帐户）。 更多信息请参阅“[{% data variables.product.prodname_dotcom %} 帐户的类型](/get-started/learning-about-github/types-of-github-accounts)”。 个人帐户拥有的仓库的所有者和协作者可以分配拉取请求审查。 具有分类权限的组织成员还可以为拉取请求分配审阅者。

要将审阅者分配给拉取请求，您需要对存储库具有写入权限。 有关仓库访问权限的更多信息，请参阅“[组织的仓库角色](/organizations/managing-access-to-your-organizations-repositories/repository-roles-for-an-organization)”。 如果您具有写入权限，则可以将具有读取访问权限的任何人分配到存储库作为审阅者。

具有写入权限的组织成员还可以将拉取请求审阅分配给对存储库具有读取访问权限的任何人员或团队。 被请求的审查者或团队将收到您请求他们审查拉取请求的通知。 If you request a review from a team and code review assignment is enabled, specific members will be requested and the team will be removed as a reviewer. 更多信息请参阅“[管理团队的代码审查设置](/organizations/organizing-members-into-teams/managing-code-review-settings-for-your-team)”。

{% note %}

**注：**拉取请求作者无法请求审查，除非他们是具有仓库写入权限的仓库所有者或协作者。

{% endnote %}

您可以向建议的或特定的人员请求审查。 建议的审查者基于 [git 追溯数据](/articles/tracking-changes-in-a-file/)。 如果您请求审查，则具有仓库读取权限的其他人仍可审查您的拉取请求。 在有人审查您的拉取请求后您做了必要的更改，您可以重新请求同一审查者再次审查。 如果请求的审查者未提交审查，并且拉取请求满足仓库的[可合并性要求](/articles/defining-the-mergeability-of-pull-requests)，则您仍然可以合并该拉取请求。

{% data reusables.repositories.sidebar-pr %}
1. 在拉取请求列表中，单击您想要请求特定人员或团队审查的拉取请求。
2. 导航到右侧边栏中的 **Reviewers（审查者）**。
3. 要向建议的人员请求审查，在 **Reviewers（审查者）**下其用户名旁边，单击 **Request（请求）**。 ![右侧边栏中的审查者请求图标](/assets/images/help/pull_requests/request-suggested-review.png)
5. （可选）要向建议人员以外的其他人请求审查，请单击 **Reviewers（审查者）**，然后单击下拉列表中的姓名。 ![右侧边栏中的审查者齿轮图标](/assets/images/help/pull_requests/request-a-review-not-suggested.png)
6. （可选）如果您知道想要其审查的人员或团队的名称，请单击 **Reviewers（审查者）**，然后输入您请求审查更改的人员用户名或团队名称。 单击其团队名称或用户名以请求审查。 ![用于输入审查者用户名的字段和带审查者姓名的下拉菜单](/assets/images/help/pull_requests/choose-pull-request-reviewer.png)
7. 审查您的拉取请求并且您已进行必要的更改后，可以请求审查者重新审查您的拉取请求。 导航到右侧边栏中的 **Reviewers（审查者）**，然后单击您想要其审查的审查者姓名旁边的 {% octicon "sync" aria-label="The sync icon" %}。 ![重新审查右侧边栏中的同步图标](/assets/images/help/pull_requests/request-re-review.png)

## 延伸阅读

- “[关于拉取请求审查](/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews)”
