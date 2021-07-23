# Guidelines to Ccontribute to IBM Cloud modules

Please take a moment to review this document in order to make the contribution
process easy and effective for everyone involved.


## Using the issue tracker

The issue tracker is the preferred channel for [bug reports](#bugs),
[features requests](#features) and [submitting pull
requests](#pull-requests).

NOTE: Please **do not** use the issue tracker for personal support requests.

<a name="bugs"></a>
## Raise an issue

Valid bugs help us to improve IBM Cloud modules and thanks for raising the same.

Guidelines for bug reports:

1. Check if the issue has already been reported.

2. Try to reproduce it using the latest `master` branch in the repository.

3. If issue still persist in latest master branch, use `issue templates` to raise a bug


<a name="features"></a>
## Feature requests

Feature requests are welcome. Please provide as much detail and context as possible. Use `feature request templates` to raise a request.


<a name="pull-requests"></a>
## Pull requests

Please adhere to the coding conventions used throughout a project (indentation,
accurate comments, etc.) and any other requirements (such as test coverage).

Follow this process if you'd like your work considered for inclusion in the
project:

1. Fork the project, clone your fork,
   and configure the remotes:

   ```bash
   # Clone your fork of the repo into the current directory 
   git clone https://github.com/<your-username>/<repo-name>
   
   # Navigate to the newly cloned directory
   cd <repo-name>
   
   # Assign the original repo to a remote called "upstream"
   git remote add upstream https://github.com/<upstream-owner>/<repo-name>
   ```

2. If you cloned a while ago, get the latest changes from upstream:

   ```bash
   git checkout <dev_branch>
   git pull upstream <dev_branch>
   ```

3. Create a new topic branch (off the main project development branch) to
   contain your feature, change, or fix:

   ```bash
   git checkout -b <topic-branch-name>
   ```

4. Commit your changes in logical chunks. Use Git's
   [interactive rebase](https://help.github.com/articles/interactive-rebase)
   feature to tidy up your commits before making them public.

5. Locally merge (or rebase) the upstream development branch into your topic branch:

   ```bash
   git pull [--rebase] upstream <dev-branch>
   ```

6. Push your topic branch up to your fork:

   ```bash
   git push origin <topic-branch-name>
   ```

7. Open a pull request with a clear title and description.

8. Make sure the github workflows are succefully running over the PR.

**IMPORTANT**: By submitting a patch, you agree to allow the project owner to
license your work under the same license as that used by the project.
