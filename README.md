# GitHub workshop sandbox

This is the practice repository for **Traceable Research Workflows with GitHub**, Session 2 of the WFDA AI Training Series at the International Water Management Institute (IWMI), held on 25 November 2026. You will make your own copy and practise one full change in it, from start to finish. It also shows how a well-set-up research repository looks, and you can reuse its templates in your own projects.

> **Your copy is public.** Anyone on the internet can see it. Do not put anything real in it: no real data, no passwords, no personal information. You can use a first name or a made-up name in the exercise.

## Hands-on exercise

You do everything in your web browser. Nothing needs to be installed.

1. **Make your own copy.** Go to <https://github.com/iwmihq/github-workshop-sandbox>. Click **Use this template**, then **Create a new repository**. Choose your own account as the owner, keep the name, choose **Public**, and create it. The next steps all happen in your copy. Check that the name at the top of the page starts with your username.

2. **Create a branch.** A branch is a separate line of work, so your change does not touch the main version until you are ready. Click the branch dropdown above the file list (it says `main`). Type `add-yourname`, for example `add-amina`, and choose **Create branch**.

3. **Edit the file.** Check that the branch dropdown now shows your branch. Open the `data` folder, then `participants.csv`. Click the pencil icon to edit. Click at the end of the last line, press Enter, and add one row about yourself:

   ```
   Your name,Your office,Your research area,A dataset you use
   ```

   Two rules:
   - No commas inside a value. Write `Flood and drought monitoring`, not `Flood, drought monitoring`.
   - Your row goes on a new line at the bottom.

4. **Commit.** A commit is a saved change with a note attached. Click **Commit changes**. Write a message that says what changed and why, for example `Add Amina to participants list for the workshop exercise`. Make sure it commits to your `add-yourname` branch, then confirm.

5. **Open a pull request.** A pull request asks for your branch to be added to `main`, and gives others a place to comment first. Open the **Pull requests** tab and click **New pull request**. Choose your branch to compare with `main`, then create the pull request. A description is filled in for you: complete the short parts. There is no issue for this exercise, so delete the `Closes #` line.

6. **Review with your partner.** Copy the link to your pull request and post it in the Teams chat. Open your partner's link, look at the **Files changed** tab, and leave a comment. Not sure what to look for? Use the [code review checklist](Code_review_checklist.md).

7. **Merge and tidy up.** Once your partner has commented, go back to your pull request. Click **Merge pull request** and confirm. Then click **Delete branch**. Open `participants.csv` on `main`: your row is there.

### Where is "push"?

In the browser there is no push step. A commit made on github.com is already on GitHub. When you work on your laptop with GitHub Desktop or VS Code, your commits stay on your laptop until you **push** them. So on a laptop there is one more step: commit, then push.

## If you get stuck

- **There is no pencil icon, or GitHub offers to "fork" the repository.** You are in the original repository, not your copy. Go to your own profile, open your copy, and try again.
- **You committed to `main` instead of your branch.** No harm done. Create your branch now (step 2), make a small edit to your row on that branch, and carry on from step 4.
- **Your row looks wrong: joined to the row above, or with too many columns.** Edit the file again on the same branch and commit. Your pull request updates by itself.

## What is in this repository

| File | What it is for |
| --- | --- |
| `data/participants.csv` | The file you edit in the exercise |
| `.gitignore` | Lists files that should never be uploaded, such as passwords and temporary files |
| `LICENSE` | Says how others may reuse the work |
| `CITATION.cff` | Tells others how to cite the work |
| `.github/` | Templates that fill in new pull requests and issues for you |
| [`templates/README_TEMPLATE.md`](templates/README_TEMPLATE.md) | A README to copy into your own project |

## After the session

**Assignment.** Within one week, apply the same steps to a real project:

1. Request a repository from the ICT helpdesk: [request guide link].
2. Add a README, using [`templates/README_TEMPLATE.md`](templates/README_TEMPLATE.md).
3. Add a `.gitignore` and a licence.
4. Open three issues, each with a label.
5. Merge one change through a pull request that closes one of the issues.
6. Tag a release called `v0.1.0`.

The usage guide explains each step: [usage guide link].

**Where to get help**

- Repositories and access: the ICT helpdesk.
- GitHub questions, deployment and hosting: Emmanuel Jolaiya, E.Jolaiya@cgiar.org, or ask in [Teams channel].
