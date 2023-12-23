# Commit writing guidelines

## The importance of Git workflow standards in the development process

The importance of standards within a team lies in their ability to provide a clear and accurate understanding of
handling specific components in the development process.
Working with the version control system Git essentially constitutes an established standard in the development world.
Crucial processes such as Code Review, CI/CD, and overall team development are built upon Git.
Rules and agreements serve as a foundation, and the better they are established, the stronger the structure's stability.
Similarly, within a team, rules and agreements regarding Git form the foundation for many team processes.
The better they are deliberated and established, the faster the team can progress.

So, what makes up Git workflow standards? Git workflow standards can be roughly divided into two groups:

- The first group builds upon Git itself, such as project management models (Git Flow, GitHub Flow, Trunk Based
  Development), agreements regarding Code Review, and creating pull requests.
- The second group is formed through practices (writing commits, setting tags, maintaining changelogs).

Here, one can observe the correlation that the more integrated a process is with team collaboration, the more important
it becomes.
This means that processes like writing commits and maintaining changelogs should be automated and take up as little time
as possible, enabling developers to focus on more critical tasks.
Here, we recall the importance of standardization since it forms the basis for automating Git workflows. Establishing
and adhering to such standards enhances team collaboration and makes other processes—such as Code Review, CI/CD, and
automatic version control—more understandable and straightforward for the entire team.

## What commit message standards do we use?

This project follows the Gitmoji standards to create clear and informative commit messages.
We use Gitmoji emojis to indicate the type of change in the commit. You can find the full
list [here](https://gitmoji.dev/)

We also strive to adhere to the commit message style convention. It encompasses seemingly minor details such as the
maximum length of the commit body, character casing, mandatory and optional components, and whether a period should be
placed at the end of the commit message. Also in your commit messages should detail why you made your change in addition
to what you did (unless it is a tiny change).

## Validation and verification of commits according to standards

Commit verification is crucial for maintaining consistency and structured history of changes in our team's projects. We
utilize [Commitlint](https://github.com/conventional-changelog/commitlint), which ensures uniformity in the commit
message format, thereby enhancing readability and aiding in
better understanding the introduced changes. Its rules help catch commit message writing errors both at the time of
creation and upon committing.

## Contribution of each team member

When adhering to commit standards, every developer in our team plays a role in maintaining and upholding these
standards. Well-structured and clear commits help us better understand the project's history, ease code reviews, and
contribute to efficient development.

We strive to maintain commit standards and utilize version control tools to ensure our projects are better structured,
more manageable, and foster effective collaboration among all developers.