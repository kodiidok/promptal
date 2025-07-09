The commands you mentioned:

```bash
git config user.name "Your Name"
git config user.email "your.email@example.com"
```

**configure the user and email *locally* (only for the current repository)** — **as long as** you're inside a Git repository when you run them.

---

### 🔍 Here's how it works:

* When run **inside a Git repo**, these commands modify the local `.git/config` file.
* If you wanted to set them **globally**, you'd add the `--global` flag:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

---

### ✅ Summary:

| Scope  | Command Example                 | Applies To                    |
| ------ | ------------------------------- | ----------------------------- |
| Local  | `git config user.name`          | Current repo only             |
| Global | `git config --global user.name` | All repos (unless overridden) |
| System | `git config --system user.name` | Entire machine (rarely used)  |

Let me know if you'd like to make this user the default globally or just in select repos.
