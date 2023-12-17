# Contributor's Guide

First off, thanks for taking the time to contribute!

When contributing to this repository, please first discuss the change you wish to make via issue, email, or any other method with the owners of this repository before making a change.

As a contributor, there are many ways to get involved:

- [Using the issue tracker](#issue-tracker)
  - [Issues and Bugs](#bug)
  - [Feature Requests](#feature)
  - [Issues management](#issue-assignment)
    - [Issue triaging](#issue-triaging)
    - [Issues assignment](#issue-assignment)
    - [Labeling issues](#issue-label)

- [Code Contributions](#coc)
  - [Coding style](#code-style)
  - [Submit a Pull Request](#submit-pr)

- [Release policy](#re-po)

## <a name="issue-tracker"></a> Using the issue tracker
The [issue tracker](https://github.com/UNamurCSFaculty/2324_INFOM126_GROUPE_07/issues) is the recommended platform for [reporting bugs](#bug) and [feature requests](#feature). It is tightly linked to the pull request system.


## <a name="bug"></a> Found a Bug?
Did you find a bug caused by the code in this repository?

1. Before you create an issue, take a moment to check the issue tracker. Your problem might already have been reported, and the discussion could provide information on available solutions or workarounds.

2. Verify if the issue has been resolved by attempting to reproduce it using the most recent main branch.

3. Try to isolate the problem

4. Open an issue in our [issue tracker](https://github.com/UNamurCSFaculty/2324_INFOM126_GROUPE_07/issues) with the `bug` label, following these [guidelines](#issue-bug-guidelines).

### <a name="issue-bug-guidelines"></a> Guidelines
A helpful bug report should give all the details upfront, so people don't have to ask you for more information. When reporting an issue, try to share as many details as you can. Please include at least:
* Your OS and web browser name and version.
* Any details about your local setup that might be helpful in troubleshooting.
* The version of the app you are using.
* Detailed steps to reproduce the bug.

Example:

> a brief and clear title for your bug report
>
> A summary of the issue (what you expected to see, versus what you actually saw) and environment in which it occurs. If
> suitable, include the steps required to reproduce the bug.
>
> 1. This is the first step
> 2. This is the second step
> 3. Further steps, etc.
>
> Any other relevant information.


## <a name="feature"></a> Feature requests
Feel free to suggest new features by opening an issue in our [issue tracker](https://github.com/UNamurCSFaculty/2324_INFOM126_GROUPE_07/issues) with the `enhancement` label ! Just make sure:
* that there aren't any duplicates in our [issue tracker](https://github.com/UNamurCSFaculty/2324_INFOM126_GROUPE_07/issues)
* your idea aligns with what our project is all about. It's your job to explain why your feature is a good fit. Give us lots of info and background to make your case stronger.


## <a name="issue-triaging"></a> Issue triaging
First, the project maintainers triage newly created issues, they categorize and prioritize issues based on their severity, importance, and alignment with project goals.


## <a name="issue-assignment"></a> Issue assignment
Once an issue is triaged, it may be assigned to a specific individual or team responsible for addressing it. Assignees are often individuals with expertise in the relevant area or those who have expressed an interest in working on similar tasks.


## <a name="issue-label"></a> Labeling issues
In our issue tracker, we use different labels to sort and recognize issues, please check them out [here](https://github.com/UNamurCSFaculty/2324_INFOM126_GROUPE_07/labels).



## <a name="code-style"></a> Coding style
when writing code that you are about to contribute to this project, please make sure to:
* Follow the Style Guide for Python Code ([PEP 8](https://peps.python.org/pep-0008/)) as closely as reasonable.
* Follow the [Django coding style](https://docs.djangoproject.com/en/dev/internals/contributing/writing-code/coding-style/).
* Use [EditorConfig](https://editorconfig.org/) or conform to the indentation style dictated in the .editorconfig file included in this repositoy.

## <a name="submit-pr"></a> Submit a Pull Request (PR)
Good pull requests (whether they're fixes, enhancements, or new features) focus on one thing and avoid adding commits that aren't related.

Before working on your pull request, please check the following:
* Please ask first before you start any significant pull request.
* Search our [repository](https://github.com/UNamurCSFaculty/2324_INFOM126_GROUPE_07/pulls) for related PRs that may affect your submission
* Make sure that there's an issue that explains the problem you're solving or the new feature you want to include, along with how it should work and look.

Once you've completed the steps mentioned earlier, you're all set to start working on your pull request!

Our contributors must follow the [Forking workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow) in order to submit code contributions. A step by step guide can be found [here](https://gist.github.com/Chaser324/ce0505fbed06b947d962) but the simplified steps are:

1. [Fork](https://help.github.com/articles/fork-a-repo/) this github repository.

2. Clone your fork, and configure the remotes:

   ```bash
   # Clone your fork
   git clone https://github.com/<YOUR_GITHUB_USERNAME>/2324_INFOM126_GROUPE_07
   # Navigate to your cloned local repo
   cd 2324_INFOM126_GROUPE_07
   # Assign the original repo to a remote called "upstream"
   git remote add upstream https://github.com/UNamurCSFaculty/2324_INFOM126_GROUPE_07
   ```

3. Create a new branch (off the main branch) to contain your feature, change, or fix:
   ```bash
   git checkout -b <topic-branch-name>
   ```
   We recommend following the [feature-branching](https://martinfowler.com/articles/branching-patterns.html#feature-branching) pattern for managing your branches where every feature has it's own branch.
  For branch naming we recommend following the ```<CATEGORY>-<ISSUE_NUMBER>-<DESCRIPTIVE_NAME>``` naming pattern, more info can be found [here](https://tilburgsciencehub.com/building-blocks/collaborate-and-share-your-work/use-github/naming-git-branches/#:~:text=3.-,Use%20the%20ID%20of%20the%20Issue,keep%20track%20of%20its%20progress.&text=This%20name%20indicates%20that%20the,is%20a%20work%20in%20progress.).

4. Commit your changes in logical chunks. Please adhere to the [Conventional Commits Specification](https://www.conventionalcommits.org/en/v1.0.0/)
   when writing commit messages. Use Git's
   [interactive rebase](https://help.github.com/articles/about-git-rebase/)
   feature to tidy up your commits before pushing them. Make sure to follow the [Coding style](#code-style).

5. Locally merge (or rebase) the upstream development branch into your topic branch:

   ```bash
   git pull [--rebase] upstream main
   ```

6. Push your topic branch up to your fork:

   ```bash
   git push origin <topic-branch-name>
   ```

7. [Open a Pull Request](https://help.github.com/articles/about-pull-requests/)
    with a clear title (following this convention ```[Issue Number] Brief and Descriptive Title```) and description against the `main` branch. (Optional) Please make sure that "allow edits from maintainers" is enabled. Your pull request will be merged once:
    * The PR checks which include tests and lint checks are passing.
    * The PR has no merge conflicts.
    * The PR has test(s) for features or enhancements. Tests for bug fixes are also appreciated as they help prevent regressions.
    * The PR is reviewed and deemed ready for merge.

Our project uses a `Squash & Merge` policy which results in your entire PR being a single commit on the main commit history.

## <a name="re-po"></a> Release policy
### Release pattern
Our project adheres to [Semantic Versioning (SemVer)](https://semver.org/) to provide a clear and standardized release pattern for our users. Semantic versioning follows the format MAJOR.MINOR.PATCH, with the following guidelines:

1. **Major Releases (X.y.z):** Major releases include significant new features, breaking changes, or major improvements.

2. **Minor Releases (x.Y.z):** Minor releases introduce new features, enhancements, or improvements without breaking existing functionality.

3. **Patch Releases (x.y.Z):** Patch releases are focused on bug fixes, security patches, and minor improvements.

### Release frequency

1. **Major Releases:** occur approximately every 6 months.

2. **Minor Releases:** are scheduled approximately every 2 months.

3. **Patch Releases:** are released on an as-needed basis, addressing critical issues promptly.
