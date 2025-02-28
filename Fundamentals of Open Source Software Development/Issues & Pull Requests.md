📌 Issues & Pull Requests (PRs) - Complete Guide
================================================

📌 Issues
---------

Used for tracking bugs, enhancements, and discussions.

-   Helps organize and manage tasks in a repository.
-   Can be manually or automatically linked to PRs for better traceability.

### **🔹 How to Create an Issue**

1️⃣ Navigate to the repository on GitHub.\
2️⃣ Click on the **"Issues"** tab.\
3️⃣ Click **"New Issue"**.\
4️⃣ Add a **title** and **detailed description** (including screenshots or code snippets if needed).\
5️⃣ Optionally, assign labels, projects, or milestones.\
6️⃣ Click **"Submit new issue"**.

* * * * *

📌 Pull Requests (PRs)
----------------------

Proposed code changes submitted by contributors.

-   Enables **code review**, discussion, and refinement before merging.
-   PRs can automatically close linked issues when merged.

### **🔹 How to Raise a Pull Request (PR) in GitHub**

#### ✅ From GitHub UI:

1️⃣ **Fork & Clone the Repository** (if contributing to an external repo):

-   Click **Fork** (top-right) → Clone the repo using `git clone <repo-url>`.\

2️⃣ **Create a New Branch**:

`git checkout -b feature-branch-name`

3️⃣ **Make Your Changes** & **Commit**:

`git add .
git commit -m "Added feature XYZ"`

4️⃣ **Push the Changes to Your Fork**:

`git push origin feature-branch-name`

5️⃣ **Open a PR in GitHub**:

-   Go to the **original repository** → Click **"Pull Requests"** → **"New Pull Request"**.
-   Select your branch → Compare changes → Add description.
-   Click **"Create Pull Request"**.

#### ✅ From GitHub UI (Direct Editing):

1️⃣ Navigate to the repository and **open a file to edit**.\
2️⃣ Click the **pencil icon** to edit.\
3️⃣ Make changes → Click **"Commit changes"** (choose a new branch).\
4️⃣ GitHub will prompt to open a **Pull Request** → Click **"Create PR"**.

* * * * *

🔗 Linking Issues with PRs (Same Repo, Different Repo, Multiple Issues)
-----------------------------------------------------------------------

### **1️⃣ Closing Issues in the Same Repository**

**Keywords:**

-   `Closes #issue-number`
-   `Fixes #issue-number`
-   `Resolves #issue-number`

✅ Example:

`Fixes #42 - Updated login validation logic.`

🔹 When merged, **Issue #42** will automatically close.

### **2️⃣ Closing Issues in a Different Repository**

**Syntax:**

-   `Closes owner/repository#issue-number`
-   `Fixes owner/repository#issue-number`
-   `Resolves owner/repository#issue-number`

✅ Example:

`Fixes octocat/example-repo#123 - Updated API error handling.`

🔹 When merged, **Issue #123** in `octocat/example-repo` will close.

### **3️⃣ Closing Multiple Issues with One PR**

**Syntax:**

-   `Closes #issue1, #issue2, #issue3`
-   `Fixes #issue1, fixes #issue2`
-   `Resolves #issue1 and resolves #issue2`

✅ Example:

`Fixes #12, #15, and #20 - Optimized database queries.`

🔹 When merged, Issues **#12, #15, and #20** will automatically close.

### **4️⃣ Linking PR to an Issue Without Closing It**

If you **don't want to auto-close** an issue, mention it **without closing keywords**:

✅ Example:

`This PR addresses issue #50 but requires further testing.`

🔹 **Issue #50 remains open** after merging.

* * * * *

📌 Manually Linking PRs to Issues in GitHub UI
----------------------------------------------

1️⃣ Open the Pull Request.\
2️⃣ Find the **"Development"** section in the right sidebar.\
3️⃣ Click **"Link issues"** and select the relevant issue(s).

* * * * *

✔ Best Practices
----------------

✅ Always use **clear commit messages** with issue references.\
✅ Link PRs to relevant issues for **better tracking & automation**.\
✅ Regularly review **open issues & PRs** to maintain project health.

* * * * *

🔗 **More Info:**

-   [GitHub Docs: Linking PRs to Issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)
