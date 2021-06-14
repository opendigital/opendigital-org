# 📘 GitLab Handbook: Always start with an issue
source: https://about.gitlab.com/blog/2016/03/03/start-with-an-issue/


## How to find the issue 


**Mar 3, 2016** - [**Heather McNamee**](https://about.gitlab.com/company/team/#nearlythere)

“Always start with an issue” says [Job](https://twitter.com/Jobvo), VP of Product here at GitLab. Before you begin anything else, summarize your ideas in an issue and share it. It’s such a simple rule, but the impact is huge.
In this post we'll focus on issues for feature proposals specifically, but the rule applies in any case, no matter what kind of project you're working on. We say “start” with an issue and not “create” an issue, because one might already exist. Make sure to search in All issues (open and closed) to see if your idea has been proposed already.


**GitLab is a discussion about software**
The benefits of collaboration start at the point of [making an issue](http://doc.gitlab.com/ce/gitlab-basics/create-issue.html). By making an issue, you get your ideas out there, and this allows your collaborators to have their say early in the process.
Non-programmers think that programmers are constantly tapping away at their keyboards on code. In fact software development is more like a discussion, and it’s a more collaborative experience than it is a solitary one.

The tools GitLab provides make it easier to manage that discussion, and keep the flow of conversation moving.

**An example of software as a discussion**
Let’s look at an example discussion as it took place around a specific feature proposal. Of course not every aspect of collaboration is recorded on GitLab. We also use text chat and we pop open a quick video chat sometimes. However, the issue tracker does give us insight into the collaborative experience.
In his recent [blog post about the Todo feature](https://about.gitlab.com/2016/03/02/gitlab-todos-feature-highlight/), GitLab developer [Douglas](https://twitter.com/dbalexandre) told the story of how the Todo feature came to be in GitLab 8.5.
The [original issue](https://gitlab.com/gitlab-org/gitlab-ce/issues/2425) was posted 6 months before coding began. The targeted milestone was moved from 8.4 to 8.5 during that time. The discussion continued for four months until the description was simplified. One of our designers, Andriy, came up with a second design reflecting the major decisions. The title changed seven times until finally it’s renamed Todos. There were 30 participants marked in the issue, but some may have just been watching, or may have taken other actions such as adding a label. In total, 13 people added to the discussion.
At one point early on, Job summarized [the next actions to take](https://gitlab.com/gitlab-org/gitlab-ce/issues/2425#note_2070496) and assigned them:

- formal proposal (Job / Darby / other people)
- mockups (Job)
- design (Andriy)
- implementation (any dev) (*which turned out to be Douglas*)

Implementation is a *final* step.
Let's consider the lifetime of this issue which started 174 days before the final release.
The task was assigned to Douglas only on Feb 2nd, with 20 days left to that milestone. Douglas spent 11% of lifetime of this issue on implementation. He didn't create the merge request until 7 days before the release. That means over the course of the issue from start to close, *only 4% of the lifetime of the issue was spent "coding".* Douglas even spent the first week of implementation reading code and writing a proposal for how he would implement the feature.
It’s in [the merge request](https://gitlab.com/gitlab-org/gitlab-ce/merge_requests/2817) that Douglas and Douwe worked on refining edge cases. They worked out how it would get done according to the intention of the original issue. Each day, Douglas would make a number of commits, and then Douwe would give him feedback. Again, it's further evidence that the bulk of work is in discussion and communication.
Of course, the Todo issue might be an extreme case, but it does highlight that software development is a discussion. Git commits themselves are just one aspect of the work software developers do. That is why tracking "commits" as evidence of productivity gives an inaccurate metric of software development productivity.

## What happens if you don’t make an issue first?

There’s a danger with spending a lot of time working on your own, before sharing the idea. As you develop it, and polish it, you run the risk of becoming too attached to it.
When you present your polished prize, you risk spending more time justifying your decisions, such as why you didn’t do X or didn’t account for Y.
By starting with an issue you also avert a number of risks which can introduce problems later on.

- You may not know everything there is to consider.
- There may be parts of the system you aren’t familiar with.
- There may be limitations or possibilities you’re not aware of.
- There may be factors for users you may not know.
- There may be work going on in a parallel effort which relates your idea.

The issue opens the conversation, and you gain the benefits of collaboration from the start.

## What's contained in the initial issue for a feature proposal?

In the [contribution guide](https://gitlab.com/gitlab-org/gitlab-ce/blob/master/CONTRIBUTING.md#feature-proposals), we call these "feature proposals" rather than "feature requests". This is a subtle but important nuance.
A 'request' puts the onus on someone else to "fulfill" a request. Whereas a 'proposal' puts the onus on the initial person writing the issue.

> Please keep feature proposals as small and simple as possible, complex ones might be edited to make them small and simple. For changes in the interface, it can be helpful to create a mockup first. If you want to create something yourself, consider opening an issue first to discuss whether it is interesting to include this in GitLab.

The Todo issue started with a [long description](https://gitlab.com/gitlab-org/gitlab-ce/issues/2425#old-deprecated-proposal-too-complex) which was later marked as "too complex". Thankfully it was kept and we can compare it.

## Are there times you don’t start with an issue?

Sure! When I’m working on something small, corrections or typo fixes, I don’t make an issue. Job said he also doesn't always make an issue. "For super small changes that don’t need to be discussed, for spontaneous outbursts of code or creativity or when you just can’t be bothered," Job said. We have to be practical, as with most rules, there are reasonable exceptions.
The [Merge Request (MR)](http://doc.gitlab.com/ee/gitlab-basics/add-merge-request.html) has everything we need anyway. MRs have the same collaboration tools as issues.

- Labels and Milestone
- Notifications
- References
- Todo notifications

So this means I can still continue the conversation. Of course, I keep the MR in ["WIP" mode](http://doc.gitlab.com/ce/workflow/wip_merge_requests.html) (work in progress) so it doesn't accidentally get merged. Then we're free to collaborate.

## GitLab workflow

So you've started with an issue, what happens next? In our next webcast on March 10th, we'll dig into a typical GitLab workflow. This will take you through the steps of making an issue, merge requests, and using tools in GitLab for cross-referencing and keeping your issue tracker organized with labels and milestones.

- Date: Thursday, March 10, 2016
- Time: 5pm (17:00) UTC; 12pm EST; 9am PST

Can't make it? Register anyway, and we'll send you a link to watch it later!
You might be curious what it's like to work remotely at GitLab. Watch this video to hear from our team!
**Our handbook**
The Remote manifesto outlines the over-arching principles. Yet it's the [handbook](https://about.gitlab.com/handbook) that details the specifics.
[The communication guidelines](https://about.gitlab.com/handbook/communication) in the handbook are thorough. My friend asked me how I could possibly remember it all. In fact you don't have to. When you start out at GitLab, you read the handbook, but you still act and react with your old habits. Luckily your colleagues will remind you, and help you learn how to *be more GitLab.*
A typical thing is to see someone say "I'm going out for lunch." But you don't need to tell people at GitLab you're going AFK (away from keyboard). So invariably, someone else will remind them: Hey no one is checking up on you.
As the handbook says:

> Everyone at the company cares about your output. Being away from the keyboard during the workday, doing private browsing or making personal phone calls is fine and encouraged.

You're expected to get your work done, and organize your own time. We do keep a group availability calendar, so if someone is away everyone can see easily.
Another typical thing is to be chatting 1:1 with someone, and someone else will say: Hey we should bring this to a group channel so others can see.
As the handbook advises:

> If you use chat please use a public channel whenever possible, mention the person you want to reach if it is urgent. This ensures it is easy for other people to chime in, and easy to involve other people, if needed.

Many rules of communication in face to face offices are implicit. Having the Handbook helps making those rules explicit and clear.
**So what has changed? The team call got bigger.**
In July 2014, Job wrote about [how GitLab works remotely](https://about.gitlab.com/2014/07/03/how-gitlab-works-remotely/). We still do have a daily [team call](https://about.gitlab.com/handbook/communication/#team-call). The technology may have changed, but that isn't as relevant as how we do it.
The rules, according to the [the Remote Manifesto](https://about.gitlab.com/2015/04/08/the-remote-manifesto/) are the same, but we had to make some changes to accommodate a larger group.
We still keep a running agenda, which acts like an internal "GitLab News" update. It's expected that even if you can't make the meeting, you still read it. We start with agenda items which anyone can add.
Then we get an update from members of a functional team. So you can find out what other teams are working on easily and ask questions. Our Marketing team gives an update on Mondays!
We still use the time for bonding too. This is one of my favorite guidelines in the handbook:

> Having pets, children, significant others, friends and family visible during video chats is encouraged. If they are humans, ask them to wave at your remote team member to say ‘Hi’.

As a remote employee since 2009, I can't even tell you how much this means to me. It reflects the human and compassionate side of GitLab. It's lovely. It's not unusual to have some small kids on laps, or dogs, or cats. The daily team meeting is meant to be a relaxing time, and it always cheers me up!
The main difference is that now we can't hear from everyone each day, so we have people grouped to speak on a specific day. Then each person talks about something they did recently, or they are planning to do. No one expects you to be "interesting" though. Whether you baked a cake or watched a movie, it's been an easy way to get to know people across the company. I was worried my nights of knitting might be boring news, but I flash a WIP (work in progress in Knitting terminology, and [on GitLab](http://doc.gitlab.com/ce/workflow/wip_merge_requests.html)) once in a while, and it's nice to share.
**How remote bonding works even better**
My favorite quote from the video above is what [Ashley](https://twitter.com/theunquietone) said: "You really get to know people and you don’t realise that you do." That's exactly how the team meeting works.
I have a feeling that I know my colleagues in this company even better than I did in previous companies. Though I haven't met any of them in person (yet!)
In an office, you might bond more easily with those in close physical proximity. With the team meeting, I feel somehow *close* to the people who joined around the same time as me. [Jose](https://twitter.com/random_primate) joined right before me, and speaks before me in the team meeting, and [Grzegorz](https://twitter.com/GrzegorzBizon) joined after me, and I hand over the call to him right after me. While we don't work on the same teams, I've become more familiar with them somehow.
The notion of *proximity* is different in a remote organization.
One day, one of our colleagues said he was really bummed out and didn't even feel like working. Everyone rallied around him. They encouraged him with positive feedback. They encouraged him to take time off too.
I kept on thinking that if this had happened in an office, he might be on the other side of the building, struggling and I wouldn't know. The lack of physical proximity has the potential to bring us closer, as long as we are sharing what we're experiencing. While it took some bravery for him to share that, I love that he did.
I know that in a way, being remote is a challenge. I can't go make him a cup of tea and chat with him. But it gives an advantage in that we all share these experiences together.
Of course, when we do get together, we can pick up where we left off. And I'm very much looking forward to that.
We have a [visiting grant](https://about.gitlab.com/handbook/incentives/#visiting-grant) at GitLab, to bring people together.

> If you want to visit a colleague in another part of the world, or promote GitLab at events in another country, then present your travel plan to your manager or the CEO, and you can receive up to $2,000 in support for your plan!

While we don't have an office, we can get financial support to visit colleagues. I'm super excited about this! I can't wait to make a trip on this grant :)
**Join us!**
Having the handbook out there in the open makes it easier for people to identify if they'd be a fit for our team.
If you'd like to work with us at GitLab, please check out the [Jobs](https://about.gitlab.com/jobs) available.

