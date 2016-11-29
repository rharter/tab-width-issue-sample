# Tab Width Issue

According to the [Material Spec](https://material.google.com/components/tabs.html#tabs-specs), when using scrollable tabs, "the width of each tab is independently calculated."  Using the design support library, this isn't the case for tablets.

This project demonstrates the issue.  It uses the scrollable fragments template project, and simply adds a `TabLayout` set to `scrollable` and tabs with variable name lengths.

When run on phones, the tabs size appropriately, but on tablets, while they're still scrollable, the tabs have the width of the longest tab name, which creates the appearance of inconsistent spacing.