# ✅ Pull Request (PR) Review Guidelines

## 🎯 1. Review the PR Description
Ensure the PR text is clear and meets these standards:
- 📋 **Purpose**: Clearly states the goal of the PR (bug fix, feature addition, refactor, etc.).
- 🔗 **References**: Links to related tickets, issues, or documentation.
- 🚦 **Checklist**: Includes any relevant notes on testing, dependencies, or manual steps required.
- ❓ **Clarity**: The description should be easy to understand, with no ambiguous language.

---

## ✅ 2. Verify Pre-Merge Tasks
Before diving deeper, ensure all automatic checks and tasks have passed:
- ✅ Linting
- ✅ Unit tests
- ✅ Integration tests
- ✅ Build checks (if applicable)

---

## 🔄 3. Pull Latest Changes
Make sure you are reviewing against the most recent version of the development branch:
```bash
git checkout dev
git pull origin dev
git checkout <pr-branch>
git rebase dev
```

---

## 🐛 4. Review the Bug/Feature Ticket
- 🔍 Confirm the PR accurately addresses the linked ticket.
- ✅ The scope of the changes matches the ticket's description.
- 📝 Any relevant documentation updates are included (if needed).

---

## 🛠️ 5. Re-Create the Bug (For Bug Fixes)
- ❌ Reproduce the issue described in the ticket.
- ✅ Verify that the PR branch resolves the bug.

---

## 💻 6. Install and Test the PR Branch
- 🏃‍♂️ Run the application using the PR branch.
- ✅ Test the **new functionality** or verify the **fix** works as expected.
- 🧪 Confirm that no existing functionality is broken.

---

## 📐 7. Verify Code Standards & Best Practices
Ensure the code follows general best practices:

### **Code Quality**
- 🔤 Clear, self-explanatory variable and function names
- 📜 Comments for complex logic
- ✂️ Avoid unnecessary code or duplication

### **Performance**
- ⚡ Efficient logic with minimal complexity
- 🚀 No unnecessary API calls or database queries

### **Security**
- 🔒 Proper validation and sanitization of input
- ❌ No hardcoded credentials or sensitive data

### **Consistency**
- 📚 Follows the project’s coding style and formatting rules
- 🏷️ Proper use of naming conventions and file structures

### **Testing**
- ✅ New features or fixes have relevant test cases
- 🧪 No broken or failing tests

### **Documentation**
- 📖 Inline comments for complex logic
- 📝 Updates to README or internal documentation (if applicable)

---

## ✅ 8. Final Approval
- 🔄 Verify the PR is up to date with the base branch (`dev`).
- 🏁 Confirm all changes meet project requirements and quality standards.
- 🛑 Approve or request changes based on your review.

