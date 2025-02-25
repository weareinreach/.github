## Summary
The following is a general suggestion of how to go about making code changes. These changes can include bug fixes, new features, refactoring, etc. This is only one way of working and is meant to be a guide to help you figure out a way that works best for you.

## Details

### 1. Understand the Product You Will Be Changing
- **Who uses this product?**
- **How do they use it?** What are the workflows and use cases?
- **Practice using it yourself.**

### 2. Understand the Change You Will Be Making
- **Understand the change request in context.** Don’t rely on your own interpretation of the change.
- **Review the request in terms of workflows and use cases.**
- **Ask questions:**
  - If you're unclear about the request.
  - If you think you're clear about the request (use your own words to describe the problem you’re being asked to solve and understand why it’s a problem).

### 3. Before Changing Anything, Research/Determine the Part of the Code That Needs to Be Changed
- **Find the code itself:** In plain English, summarize what this code is doing.
- **What other areas of the app rely on this piece of code?**
- **Look for the existence of unit tests.**
- **Run the unit tests locally:**
  - Is this part of the code being fully tested?

### 4. Determine How You Can Implement the Change
- **In plain English, explain your intended change and organize your thoughts.**
- **Create a list of changes you will need.**
- **Write pseudocode if necessary.**
- **Keep it simple:** Choose the least convoluted means to achieve the desired results. Remember that it is often more important to "make it work" than to try to make something future-proof.
- **Think about what areas of the app can be impacted by this change.**
- **Determine how you would test this.**

## Getting Ready to Code
This section is more specific to InReach and the process used by the development team.

1. **Ensure there is an ticket for the request.**
   - This should have all the information you need to do the work. If it lacks details, ask questions and add the missing information to the ticket.
   - Having the information in the ticket ensures all members of the team will have access to the details of the requested change.
2. **Capture use cases and workflows in the ticket.**
3. **Capture exceptions in the ticket.**
4. **Include links to design mock-ups if they exist.**
   - Include anything and everything you find while researching this task.
5. **Add sub-tasks or just break it down as bullet points, to the ticket.**
   - Sub-tasks are the steps you've determined in step 4 above.
   - Ideally, a sub-task should be self-contained and not rely on other code changes to function.
   - Be sure to include updating/creating unit tests.

## Making the Change

1. **Create a branch that references the ticket number.**
   - Almost always, you will base this on the `dev` branch. It’s rare that you’ll make a hotfix off the `main` branch.
2. **Ensure the code runs.**
   - Before making any changes, ensure the branch you just created can run the code (app, control-panel, or API).
   - Run the unit tests and ensure they pass.
3. **Make your first change.**
   - Keep it simple.
4. **Commit it.**
5. **Push it to GitHub** (on your feature branch).
6. **Update often:** Push your changes to GitHub as you complete each task.
   - Push your changes to GitHub on the branch you created to track these changes.

## Preparing to Submit a PR

1. **Test your code changes locally.**
   - Run tests manually.
   - Run unit tests with and without the UI (headless).
2. **Fix any tests that fail and update GitHub.**
3. **Submit a PR.**
   - Ensure the PR is against the correct branch (most likely `dev`).

## PR Follow-Up

- Be prepared to address any issues that arise during the review/approval process.
