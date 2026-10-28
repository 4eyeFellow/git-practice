# Reflection

**1. Why is Squash and Merge better for small feature branches?**
It turns all the little commits on a branch into one clean commit on main. That way main isn't cluttered with stuff like "fix typo" or "wip," and it's easy to see what each feature added.

**2. What's the difference between "Add single comment" and "Start a review"? Why batch?**
Add single comment posts each comment right away and sends a notification every time. Start a review saves all your comments and sends them together, so the author gets one notification and sees all the feedback at once instead of getting spammed.

**3. How do Branch Protection Rules prevent production breakage?**
They block anyone from pushing straight to main, so every change has to go through a pull request and get reviewed first. That gives you a chance to catch bugs before they hit the main code.

**4. Why merge origin/main into your feature branch locally instead of force pushing?**
Merging locally lets you see the conflict, pick the right code, and test it before pushing. Force pushing can wipe out other people's work or history, while merging keeps everything and just updates the PR.