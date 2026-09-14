# In-Class 1 v3 — Reinforcement Edition

## Team Members

* Greena Patel
* Anuradha


## Widget Tree

In Flutter, everything displayed on the screen is a widget. Widgets are placed inside other widgets, which creates a tree structure. In our tabbed application, the `Scaffold` contains the `AppBar`, `TabBarView`, and `BottomAppBar`. Each tab also contains its own widgets such as buttons, text fields, cards, and lists.

## Stateless vs. Stateful Widgets

A `StatelessWidget` is used when the widget does not need to store changing information. A `StatefulWidget` is used when the application needs to remember or update information while it is running. For example, keeping track of the selected tab requires state.

## Controllers and Lifecycle

Controllers help manage widgets that need additional control, such as a `TabController`. The controller can be created inside `initState()` when the widget starts. It should be cleaned up inside `dispose()` when the widget is removed. This helps prevent unnecessary memory usage and memory leaks.

## Declarative UI

Flutter uses a declarative approach to build user interfaces. Instead of manually changing individual widgets, we update the state and Flutter rebuilds the parts of the interface that need to change. The `build()` method describes what the UI should look like based on the current state.

## GitHub Collaboration

For this activity, we practiced working together using a shared GitHub repository. Each team member worked on a separate branch, made their own commits, pushed their work to GitHub, and created a pull request. We also reviewed each other's changes and left comments before merging the pull requests into the `main` branch.

This workflow helped us understand how developers collaborate on the same project without directly changing the main branch.

## Greena's Individual Reflection

This activity helped me understand the Flutter concepts from our previous tabbed app in a clearer way. The widget tree showed me how the different parts of the interface are connected through parent and child widgets.

I also learned why some widgets need to be Stateful while others can remain Stateless. If a widget needs to remember or update information, such as the currently selected tab, it needs state.

The lifecycle section also helped me understand why controllers should be created and cleaned up properly. Using `dispose()` is important because it prevents unused resources from remaining in memory.

I also learned how GitHub collaboration works in a team. Working on a separate branch, committing my own changes, creating a pull request, and reviewing my teammate's work helped me understand how developers can work on the same project without directly editing the `main` branch.

The controller is created in `initState()` because this method runs when the State object is initialized.

The controller is cleaned up in `dispose()` because it is no longer needed when the widget is removed.

Example:

```dart
@override
void initState() {
  super.initState();
  _tabController = TabController(length: 4, vsync: this);
}

@override
void dispose() {
  _tabController.dispose();
  super.dispose();
}

## GitHub Collaboration

I created a separate branch named `anuradha-notes` to work on my contribution without directly modifying the main branch. My changes will be reviewed by my teammate through a Pull Request before being merged into main.
