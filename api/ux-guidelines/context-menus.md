---
# Summarize the whole topic in less than 300 characters for SEO purpose
MetaDescription: UX guidelines for using context menus in a Visual Studio Code extension.
---

# Context Menus

[Menu items](/api/references/contribution-points#contributes.menus) appear in views, actions, and right-click menus. It's important that the grouping of menus remain consistent. If your extension has actions that relate to files, place your actions in the File Explorer context menu (when appropriate). If an extension has actions for certain file types, only display it for those items.

**✔️ Do**

* Show actions when contextually appropriate
* Group similar actions together
* Place large groups of actions into a submenu

❌ Don't

* Show actions for every file without context

![Context Menu](images/examples/context-menu.png)

*This example places a **Copy GitHub Link** next to the other copy commands. This action only appears on files that are from a GitHub repository.*