# Practitioner Guide: Contributor Sustainability

Primary metrics:
* [Bus Factor](https://chaoss.community/?p=3944)
* [Contributors](https://chaoss.community/?p=3467)
* [Types of Contributions](https://chaoss.community/?p=3432)

If you haven’t already read the [Practitioner Guide: Introduction - Things to Think about When Interpreting Metrics](https://chaoss.community/practitioner-guide-introduction/), please pause now and read that guide.

Contributor sustainability is an important part of assessing whether an open source project and community have enough contributors for the project to be sustained over the long-term, so contributor sustainability has a large impact on overall project sustainability. There are a lot of projects with a single maintainer (see [xkcd Dependency](https://xkcd.com/2347/)), and many projects struggle to find enough people to actively participate in their projects and continue to maintain them over the long term. The reality is that there are a lot of open source projects and not enough contributors, so maintainers are in desperate need for help across the various types of contributions needed to have a successful and sustainable open source project. If there are not enough contributors to sustain a project, this increases the risks that the project will fail, which creates a variety of often significant challenges for the users and other projects that depend on it.

# Step 1: Identify Trends
There are a number of things that can impact contributor sustainability. By starting with [Bus Factor](https://chaoss.community/?p=3944), you can assess the risk to the project if key contributors / maintainers decided to leave, but it’s also important to look at other trends related to [Contributors](https://chaoss.community/?p=3467) along with the [Types of Contributions](https://chaoss.community/?p=3432) that people are making to identify potential contributor risks that might impact the overall sustainability of your project.

## Bus Factor
Bus Factor is important for understanding contributor sustainability because it visualizes the question "how many contributors can we lose before a project stalls?" It helps to identify how widely the work in a project is distributed across contributors and identify the key people in a project that are doing the majority of the work. If the majority of work is being performed by a single person or small number of people, it increases the risk that a project could become unsustainable if that person or people were no longer working on the project. 

![Bus Factor bar chart with balanced contributions ranging from 16% of commits to 6% of commits](https://github.com/chaoss/wg-data-science/blob/main/practitioner-guides/images/bus-factor-bar-balanced.png "Bus Factor - generated by Augur")

## Contributors
The contributors metric looks broadly at who contributes to a project and can be visualized in many different ways. While you can look at this as a single number of contributors over time, it can help to break this down to help you understand how many contributors are active along with how many have increasing or decreasing activity over time. While the bus factor metric is good at identifying key contributors, you should also try to understand contributor sustainability more broadly to look at overall trends across all contributors to see if you are experiencing contributor growth or decline. 

![Active Contributors over time and growth analysis showing positive and negative contributor balances](https://github.com/chaoss/wg-data-science/blob/main/practitioner-guides/images/active-contrib-over-time-bar-trend.png "Active Contributors over time - generated by GrimoireLab")

## Types of Contributions
Multiple, varied contributions impact open source project health and sustainability, and contributions may include writing code, managing the community, triaging bugs, evangelizing the project, supporting users, or helping in other ways. A variety of contribution types can demonstrate that a project is mature and well-rounded with sufficient activity to sustain all aspects of the project, and enable paths to leadership that are supportive of a variety of contribution types and people with varying expertise beyond coding. 

![Contributions by Data Source for various sources over time including GitHub, Twitter, pipermail, Slack](https://github.com/chaoss/wg-data-science/blob/main/practitioner-guides/images/contrib-by-data-source.png "Contributions by Data Source - generated by GrimoireLab")

# Step 2: Diagnosis
As mentioned in the Practitioner Guide Introduction, you should start by talking to a few people who are intimately involved in the project so that you can look together at the trends and interpret them in a way that makes sense for the project. For example, the image below shows that over 60% of the commits in this project in the past year were made by a single individual, which in most cases increases the risk that the project could become unsustainable if that person or people were no longer working on the project. However, it’s also important to think about this in light of other aspects of the project. For example, if this project is mostly documentation that many people have the knowledge to update or if it’s code that is fairly simple and easy for others to understand or if the project is mostly used by a single individual, then the risk is relatively low. On the other hand, if the project is complex, large, and / or widely used, then the risk is high and the project should focus on recruiting more contributors and maintainers to increase contributor sustainability.

![Bus Factor pie chart showing that one contributor has made 61.8% of the commits with next largest contributors making 10.8% and 9.77%](https://github.com/chaoss/wg-data-science/blob/main/practitioner-guides/images/bus-factor-pie-one-person.png "Bus Factor - generated by 8Knot / Augur")

It’s also important to look at other trends related to contributors. For example, the graph below shows that active contributors peaked and then declined for this project, so it would be important to diagnose why that might be the case. If the project was something bounded in time (e.g., related to a conference or workshop) that was completed or a project where most of the work has been completed and is not being lightly maintained, this would be a normal pattern to see. However, if this is a typical open source project, this could indicate that there are serious issues impacting the retention of contributors that should be diagnosed and addressed.

![Contributor Growth by Engagement showing that the active contributors peaked in April 2023 and dwindled to nothing by October 2023](https://github.com/chaoss/wg-data-science/blob/main/practitioner-guides/images/contributor-growth-by-engagement-bar.png "Contributor Growth by Engagement - generated by 8Knot / Augur")

# Step 3: Gather Additional Data if Needed
CHAOSS has other metrics related to responsiveness that can help diagnose specific problems within your community.

Additional Metrics: 
* [Inclusive Leadership](https://chaoss.community/kb/metric-inclusive-leadership/)
* [Newcomer Experience](https://chaoss.community/kb/metric-newcomer-experience/)
* [New Contributors](https://chaoss.community/kb/metric-new-contributors/)
* [Project Burnout](https://chaoss.community/?p=3537)
* [Project Demographics](https://chaoss.community/kb/metric-project-demographics/)

# Step 4: Make Improvements
There are a couple of things that the Bus Factor can tell you that can be used to help drive contributor improvements that make your project more sustainable. First, it helps you decide how sustainable your current contributor situation is. If one person is making most of the contributions and the project is large or complex, you should focus on ways to distribute the load and have more people involved in the project. Second, the Bus Factor metric can help you find people who might be contributing more than you realized, which can help you think about who you can encourage to contribute more or maybe find someone who could move into a leadership role (e.g., reviewer or maintainer). With respect to leadership roles, you might look at someone making ten percent of the contributions and decide that they are ready to become a maintainer. One way to do this is to reduce the scope for new maintainers. If they aren’t ready to be a maintainer for the entire project, maybe they can maintain a sub-project or a specific section of the project while they build their expertise in other areas. One way to do this is by using OWNERS or [CODEOWNERS files](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners) to give people responsibility for different areas within your repository, including docs or community sections. People who are making fewer, but regular contributions might be good candidates for mentorship or becoming reviewers with an eye toward making them maintainers after they gain a bit more experience.

It’s also important to look at your contribution guides or other onboarding documentation to make sure that new contributors can easily get started within your project (see Additional Reading section for links). Good documentation is how we scale the things that take up precious time for already overworked maintainers and free up their time to work on other things. At a minimum, a new contributor needs to understand how to spin up an environment where they can do their development, the expectations for testing and how to run tests, any processes or expectations that you have for pull requests, and instructions for other requirements. If this is well documented, new contributors can get started with a minimal amount of help from existing maintainers, which can save you a lot of time in the long run. When a project doesn’t have good onboarding docs, maintainers can get frustrated by the amount of time they spend on new contributor questions, which can make it hard for new contributors to feel welcome and take a long time for them to become productive. This is how people get discouraged and drift away from your project. This doesn’t mean that you need to spend days and weeks writing perfect onboarding documents. Anything is better than nothing, and if you start with a few things that will help people get started quickly, new contributors can actually help make the onboarding documents better by adding more details and additional instructions for things that they found confusing or that they struggled with. 

Having good first issues or help wanted labels are excellent places to start because these help people find something that they can work on while they learn more about the project. Good first issues should be targeted as something simple that a brand new contributor could pick up and complete in a short amount of time to help them learn more about your contribution process. Help wanted labels can be for issues that are a little more involved so that people who have already started to contribute can find something else to work on. Good first issues and help wanted labels along with good contribution guides helps you build a sustainable pipeline of contributors for your project.

However, good first issues and help wanted labels are passive requests for help, so I also encourage maintainers to also be proactive and specific about ways that people can help. Asking someone specific to review a PR or answer a question from a user demonstrates that you recognize their unique expertise and want their help. Knowing that we’re wanted and appreciated makes us feel good, which can be a strong motivator to contribute to an open source project or to continue contributing. Reaching out to someone and acknowledging their work while encouraging them to do more can help you recruit people who could take on increasing responsibilities (e.g., reviewer or maintainer) within your project. Don’t be afraid to reach out to your power users in addition to your contributors, and if you work at a company, you can use your corporate relationships with other organizations to find people who might be interested in contributing.

Defining the roles and responsibilities for contributors, reviewers, and maintainers can help with recruiting new people into these roles. It can help to think about this as a [contributor ladder](https://github.com/cncf/project-template/blob/main/CONTRIBUTOR_LADDER.md) where contributors can climb up to become reviewers and those reviewers can become maintainers. What’s important is to document this and make sure that people understand how they can climb the ladder and gain more responsibilities within the project. Moving more people into leadership roles, like review and maintainer, can help reduce the bus factor and make your project more sustainable over time.

The catch here and with many metrics is that we don’t want to just think about people who are making code contributions. This is a good start, but you should also be thinking about how you can move people into leadership positions to be responsible for things that might not show up in GitHub or GitLab, like documentation, community management, marketing and other important roles. This is why it is so important to also look at the Types of Contributions metric. It’s common to see maintainers underestimating the amount of time spent on some of these tasks, and recruiting more people into other roles can further distribute the workload and increase contributor sustainability.

Maintainers for a project with a low bus factor, especially if they’re the only maintainer, should have some type of succession plan in place. At a minimum someone else should have admin access to everything needed to update the software and publish releases (including publishing to relevant package managers) along with documentation for how to do this. Ideally, there is another maintainer on the project who can share the responsibilities equally and already has the access, skills, and knowledge to perform all project tasks, which is one reason that the above discussions about building your contributor base and recruiting maintainers is so important. While not ideal, for single maintainer projects succession planning could include providing access and documentation to a trusted colleague or friend. The key to succession planning is to put it in place now, before you think you need it.

# Step 5: Monitor Results
How you monitor the results will depend on what improvements you decided to make. Continuing to monitor these 3 metrics are a good start. If you used other data from Step 3, you should also monitor those metrics.

If you are recruiting new contributors, approvers, and maintainers, it might take a while to see the results of those efforts, so you might not see significant improvements for 3 to 6 months, so you’ll need to monitor this over a longer period of time.

# Cautions and Considerations

* It’s critical to think about the human dynamics that can influence contributor sustainability and to treat people with kindness and respect as you work to make improvements.

# Additional Reading

* The CNCF has several [templates](https://contribute.cncf.io/maintainers/templates/) for writing a good [CONTRIBUTING.md](https://contribute.cncf.io/maintainers/templates/contributing/) guide and [Contributor Ladder](https://github.com/cncf/project-template/blob/main/CONTRIBUTOR_LADDER.md).
* The [Responsiveness Practitioner Guide](https://chaoss.community/practitioner-guide-responsiveness/) also has some similar suggestions that can apply to contributor sustainability. 

# Feedback

We would love to have feedback to learn more about how people are using the CHAOSS Practitioner Guides and how we can improve them over time. Please complete this [short survey](https://forms.gle/w3B1gBH8kp3rPbhr8) to provide your feedback.

# Contributors
The following people contributed to this guide:

* Dawn Foster
* Chan Voong
* Jeffrey Osier-Mixon
* Luis Cañas Díaz
