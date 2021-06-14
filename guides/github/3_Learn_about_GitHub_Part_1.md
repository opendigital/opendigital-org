# 3️⃣ 3. Learn about GitHub Part 1
[](https://forms.gle/9wNWQ9DMTmeHyJcL6)
**BEFORE YOU GET STARTED:**



Key Action Items



----------


## Chapter 1: Git vs GitHub
- `git` is not GitHub.com
    - explain briefly what is `git` (technical)
    - then give overview of all the activities and features of GitHub (non-technical)


----------
## Chapter 2: Workflows

**Git vs. Dropbox**

    - explain what file-synchronization (Dropbox) (technical)
    - Dropbox is effortless, automatic, and require no thought
    - These features also are what make it terrible for project work
    - `git` is purposeful, error correcting, requires some thought


**GitLab Product Handbook**
`https://about.gitlab.com/handbook/product/#enabling-collaboration`

**GitLab core team & GitLab Inc. contribution process**

> From development teams to marketing organizations, everyone needs to collaborate on digital content. Content should be open to suggestions by a wide number of potential contributors. Open contribution can be achieved by using a mergeable file format and distributed version control. The [mission of GitLab](https://about.gitlab.com/company/strategy/#mission) is to **allow everyone to collaborate on all digital content** so people can cooperate effectively and achieve better results, faster.

 
**Bringing Ideas to Reality**

> Ideas flow through many stages before they are realized. An idea originates in a chat discussion, an issue is created, it is planned in a sprint, coded in an IDE, committed to version control, tested by CI, code reviewed, deployed, monitored, and documented. Stitching together all these stages of the DevOps lifecycle can be done in many different ways. You can have a marketplace of proprietary apps from different suppliers or use a suite of products developed in isolation.

**Iteration**

> A minimum-viable-change (MVC) approach is a byproduct of our spirit of iteration. Even when not pursuing an MVC, we will encourage iteration in our own development process. That means we [break problems down](https://about.gitlab.com/handbook/product-development-flow/#build-phase-1-plan) as [small as possible](https://about.gitlab.com/handbook/values/#make-small-merge-requests), use [throughput as a performance indicator](https://about.gitlab.com/handbook/engineering/development/performance-indicators/#throughput), and focus on [reduced cycle time](https://about.gitlab.com/handbook/values/#reduce-cycle-time). Thinking iteratively is not always intuitive, and breaking certain topics or projects down can be challenging. Here's a helpful [video](https://www.youtube.com/watch?v=zwoFDSb__yM) from our CEO with guidance on how to think more iteratively.



----------


## Chapter 3: Issues

**3.1 - Issue Philosophy**

Enabling transparency and managing change in projects with collaboration

“Issues are the fundamental medium for collaborating on ideas and planning work in GitLab.”

The GitLab issue tracker is an advanced tool for collaboratively developing ideas, solving problems, and planning work.

**GitLab Project Documentation:** 
`https://docs.gitlab.com/ce/user/project/issues/`

GitHub Issues Overview:  `https://guides.github.com/features/issues/`

Issues can allow sharing and discussion of proposals before, and during, their implementation between:

- You and your team.
- Outside collaborators.

They can also be used for a variety of other purposes, customized to your needs and workflow.
Issues are always associated with a specific project, but if you have multiple projects in a group, you can also view all the issues collectively at the group level.

**Common use cases include:**

- Discussing the implementation of a new idea
- Tracking tasks and work status
- Accepting feature proposals, questions, support requests, or bug reports
- Elaborating on new code implementations


**Articles**

**“Always start with an issue” | GitLab Blog**

> “Always start with an issue” says [Job](https://twitter.com/Jobvo), VP of Product here at GitLab. Before you begin anything else, summarize your ideas in an issue and share it. It’s such a simple rule, but the impact is huge.

 - `https://about.gitlab.com/blog/2016/03/03/start-with-an-issue/`

**“Tutorial: It's all connected in GitLab” | GitLab Blog**

> In GitLab, everything you do can be cross-linked and referenced. This improves discoverability and reduces duplicate effort.
> 
> GitLab is more than just a Git repository manager. There are a number of tools to help you collaborate with others, or even just manage a project yourself. The best features of GitLab help you link and reference related work.
> 
> Your issue is the Single Source of Truth

 - `https://about.gitlab.com/blog/2016/03/08/gitlab-tutorial-its-all-connected/`

**“Almost Everything We Do Will Be Open” | GitLab Blog**
- `https://about.gitlab.com/blog/2015/08/03/almost-everything-we-do-is-now-open/`

**GitLab Company Communication Handbook**
 `https://about.gitlab.com/handbook/communication/#issues`


> Issues are useful when there isn't a specific code change that is being proposed or needed. For example, you may want to start an issue for tracking progress or for project management purposes that do not pertain to code commits. This can be particularly useful when tracking team tasks and creating issue boards. However it is still important to maintain focus when opening issues by defining a single specific topic of discussion as well as defining the desired outcome that would result in the resolution of the issue. 
> 
> The point is to not keep issues open-ended and to prevent issues from going stale due to lack of resolution. For example, a team member may open an issue to track the progress of a blog post with associated to-do items that need to be completed by a certain date (e.g. first draft, peer review, publish). Once the specific items are completed, the issue can successfully be closed. Below are a few things to remember when creating issues


**3.2 - Issue Management**

**Issue Dashboard gives an overview of all projects and open tasks**

![](https://paper-attachments.dropbox.com/s_FE414D50390C26D91A0922774D4358FD54E73D0B0DF25D27D417837C656F72D2_1585844605083_image.png)

![](https://paper-attachments.dropbox.com/s_FE414D50390C26D91A0922774D4358FD54E73D0B0DF25D27D417837C656F72D2_1585844847443_image.png)


Things you can do with the project issue tracker


- [Create an issue from a template](https://docs.gitlab.com/ce/user/project/description_templates.html#using-the-templates)
- [Set a due date](https://docs.gitlab.com/ce/user/project/issues/due_dates.html)
- [Bulk edit issues](https://docs.gitlab.com/ce/user/project/bulk_editing.html) - From the Issues List, select multiple issues in order to change their status, assignee, milestone, or labels in bulk.
- [Import issues](https://docs.gitlab.com/ce/user/project/issues/csv_import.html)
- [Export issues](https://docs.gitlab.com/ce/user/project/issues/csv_export.html) 
- Connect directly with the [Issues API](https://docs.gitlab.com/ce/api/issues.html)
- Configure an [external issue tracker](https://docs.gitlab.com/ce/integration/external-issue-tracker.html) such as Jira, Redmine, or Bugzilla



- **Milestones**
- **Labels**
- **Due Dates**
- **Assignees**
- **Notifications**
- **@mentions**
- **References**


**GitLab Engineerring Workflow Handbook**
`https://about.gitlab.com/handbook/engineering/workflow/`


Examples of collaborative team workflow and using issue trackers 

    https://gitlab.com/gitlab-org/gitlab-design/-/issues/1051
![https://gitlab.com/gitlab-org/gitlab-design/-/issues/1051](https://paper-attachments.dropbox.com/s_FE414D50390C26D91A0922774D4358FD54E73D0B0DF25D27D417837C656F72D2_1585842966159_image.png)




1. When **closing** an issue leave a comment explaining why you are closing the issue and what the MVC outcome was of the discussion (if it was implemented or not).
2. We keep our **promises** and do not make external promises without internal agreement.
3. Be proactive and consistent with communication on discussions that have external stakeholders such as customers. It's important to keep communication flowing to keep everyone up to date. Issues can appear stale if there aren't recent discussions and no clear definition on when another update will be provided, based on feedback. This leaves those subscribed in the dark, causing unnecessary surprise if something ends up delayed and suddenly jumps to the next milestone. It is important that issues are closed in a timely manner. One way of doing this is having the current assignee set a due date for when they will provide another update. This can be days or weeks ahead depending on the situation, prioritization, and available capacity that we may have.
4. If a user suggests an enhancement, try and find an existing issue that addresses their concern, or create a new one. Ask if they'd like to elaborate on their idea in an issue to help define the first MVC via a subsequent MR.
5. **Cross link** issues or MRs with related conversations. Another example is to add "Report: " lines to the issue description with links to relevant issues and feature requests. When done, add a comment to relevant issues (and close them if you are responsible for reporting back, or re-assign if you are not). This prevents internal confusion and us failing to report back to the reporters.
6. Prioritize your work on issues in the current [milestone](https://gitlab.com/groups/gitlab-org/-/milestones).
7. Use the public issue trackers on GitLab.com for everything since [we work out in the open](https://about.gitlab.com/blog/2015/08/03/almost-everything-we-do-is-now-open/). Issue trackers that can be found on the relevant page in the handbook and in the projects under [the gitlab-com group](https://gitlab.com/gitlab-com/).
8. Assign an issue to yourself as soon as you start to work on it, but not before that time. If you complete part of an issue and need someone else to take the next step, **re-assign** the issue to that person.
9. Ensure the issue **title** states what the desired outcome should be. For instance, for bugs make sure the issue states the desired result, not the current behavior.
10. **Regularly update** the issue description with the latest information and its current status, especially when important decisions were made during the discussion. The issue description should be the **single source of truth**.
11. If you want someone to review an issue, do not assign them to it. Instead, @-mention them in an issue comment. Being assigned to an issue is a signal that the assignee should or intends to work on it. So you should not assign someone to an issue and mis-represent this with a false signal.
12. Do not close an issue until it is [**done**](https://docs.gitlab.com/ee/development/contributing/merge_request_workflow.html#definition-of-done). It's okay to explicitly ask if everyone is on board and in agreement on how to move forward, whether to iterate, close the open issue, or create a subsequent MR to implement a MVC.
13. Once a feature is [**done**](https://docs.gitlab.com/ee/development/contributing/merge_request_workflow.html#definition-of-done), update the description to add a link to the corresponding documentation. When using a Search Engine, issues often appear before documentation pages, which makes it harder to find the relevant information about the feature.
14. Write issues so that they exclude private information. This way, the issue can be public. Only use confidential issues, if the issue must contain [non-public information](https://about.gitlab.com/handbook/communication/#not-public).
15. If the content within a public issue transitions to become what is deemed confidential [non-public information](https://about.gitlab.com/handbook/communication/#not-public), the issue may be made confidential.
16. If the content of a public issue draws comments that are deemed in violation of our [code of conduct](https://about.gitlab.com/community/contribute/code-of-conduct/) the issue may be locked and may [undergo moderation](https://about.gitlab.com/handbook/marketing/community-relations/community-advocacy/workflows/code-of-conduct-enforcement/#overview).



