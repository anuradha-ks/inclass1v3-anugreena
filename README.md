# In-Class 1 v3 — Reinforcement Edition

## Team Members

- Sai Anuradha Kappaganthula
- Greena Patel

---

# My Concept Notes

## 1. Widget Tree

Flutter builds the user interface as a tree of widgets. Each widget can contain other widgets, creating a parent-child relationship.

For example, a simplified structure of our app is:

MaterialApp
└── Scaffold
    ├── AppBar
    ├── Body
    │   └── TabBarView
    │       └── Tab content
    └── BottomAppBar

This structure is called the Widget Tree. Every visible part of the application is created from widgets, and Flutter uses this tree to determine what should appear on the screen.

---

## 2. Stateless vs. Stateful Widgets

A StatelessWidget is used when the widget does not need to maintain changing state.

A StatefulWidget is used when the widget needs to remember information that can change while the application is running.

Our tabbed application uses a StatefulWidget because it needs to manage changing information such as the selected tab and the TabController.

A StatefulWidget has a State object where the changing state and lifecycle-related logic are managed.

---

## 3. Controllers and Lifecycle

A controller allows the application to manage or interact with a particular widget or resource.

Our application uses a TabController to control the tabs.

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