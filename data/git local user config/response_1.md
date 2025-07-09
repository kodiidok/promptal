To locally define your Git user **just for the current repo** (without affecting the global settings), you can override the user configuration in the repository's local `.git/config`.

Here’s how to do it:

### ✅ Step-by-step Instructions

1. **Navigate to your repo directory:**

```bash
cd /path/to/your/repo
```

2. **Set your name and email for just this repository:**

```bash
git config user.name "Your Name"
git config user.email "your.email@example.com"
```

This overrides the global settings **only for this repo**.

3. **(Optional) Verify the settings:**

```bash
git config --list --local
```

You should see:

```
user.name=Your Name
user.email=your.email@example.com
```

---

### ✅ To double-check the global one isn't used:

```bash
git config --list --show-origin
```

This will show which config file each setting comes from — local or global — helping you confirm it's overridden correctly.

Let me know if you want this change to be permanent for all repos *except* one.
