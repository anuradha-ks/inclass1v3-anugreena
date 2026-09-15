# In-Class 1 v3 — Reinforcement Edition

## Student Name

Greena Patel

## Team Member

Anuradha

# Individual Reflection

## 1. What surprised you most about how the widget tree, state, or lifecycle actually behaves once you saw it applied in the app?

What surprised me the most was how everything in Flutter is connected through the widget tree. I already knew that Flutter uses widgets, but after looking at the tabbed app, I understood better how one widget is placed inside another. For example, the `Scaffold` contains the `AppBar`, `TabBarView`, and other widgets, and then each tab has its own content inside it.

I also did not realize before how important the lifecycle of a widget is. Things like controllers cannot just be created and left there. They also need to be cleaned up properly when they are no longer being used.

## 2. Which concept took the longest to click for you, and what finally made it make sense?

Controllers and lifecycle methods took me the longest to understand. At first, `initState()` and `dispose()` just felt like methods that we had to use because Flutter required them.

It made more sense once I thought about `initState()` as the place where something starts and `dispose()` as the place where it gets cleaned up. For example, the `TabController` is created when the widget starts and then disposed when the widget is removed. Thinking about it that way made the concept easier to understand.

## 3. What part of the GitHub workflow felt least familiar, and how did you work through it?

The least familiar part for me was working with branches, pull requests, and merge conflicts. I had used basic Git commands before, but working with another person in the same repository was different.

I worked on my own branch called `greena-notes`, made my changes there, committed them, pushed the branch, and then created a pull request.

We also had a merge conflict in the README because both branches had different changes in the same file. At first, the conflict markers looked confusing, but after looking at both versions, we decided what content we wanted to keep and removed the conflict markers.

I also had a push rejected because the remote branch had changes that I did not have on my computer yet. That helped me understand why it is important to pull the latest changes before pushing.

## 4. If you rebuilt this activity from scratch tomorrow, what would you do differently?

If I did this activity again, I would make sure the `main` branch was completely updated before creating my own branch.

I would also talk with my teammate before starting and decide which files or sections each person would work on. Since both of us made changes to the README, it created a merge conflict.

I would also make sure to pull the latest changes before starting new work and before pushing. I think that would make the whole process smoother.

# Peer Feedback and Reflection

## 5. Describe one specific contribution from your teammate that you found genuinely helpful, and why.

One thing Anuradha did that helped me was working on the shared repository and adding notes about the controller lifecycle.

Seeing how the `TabController` is created in `initState()` and cleaned up in `dispose()` made the idea easier for me to understand because I could connect the explanation directly to the code.

## 6. Share one piece of constructive feedback that could help your teammate collaborate even more effectively next time.

One thing we could improve next time is deciding before we start which person will work on which part of the project.

Since both of us edited the README, we ended up with a merge conflict. If we divide the work more clearly at the beginning, it would probably make the collaboration easier and avoid some conflicts.

## 7. What is one thing you learned from watching how your teammate approached a problem?

One thing I learned was the importance of working on separate branches instead of making changes directly to `main`.

Seeing how we could both work on our own branches and then combine the changes through pull requests helped me understand how developers can work on the same project without interfering with each other's work.

I also saw why reviewing each other's changes before merging is useful, even for a small assignment.

## 8. How did the two of you resolve any disagreements or merge conflicts, and what would you try differently next time?

We had a merge conflict in the README because both branches had changes in the same file. Git showed the different sections using conflict markers.

We looked at both versions, decided which parts we wanted to keep, combined the useful content, and removed the conflict markers.

Next time, I would try to avoid having both of us edit the same part of the same file at the same time. I would also make sure we both pull the newest version of `main` before starting our work. I think that would make the merging process much easier.
