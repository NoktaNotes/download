v0.10.0 - Solid Foundations (MY Summary)

Building an app is hard work. You add some functionality, and it sort of works. Then you redo it, redo it again, throw it all away because it turns out it's just not working. Then try it once more until it finally does what you want it to do. And then make it play nicely with the rest of the app. Create a bug list, work your way through it... And once everything in your list is solved, there is a whole new list of bugs caused by your fixes.
Build - Break - Fix - Repeat

That's why I call this release "Solid Foundations". I've gone through the cycle so many times that there's nothing major on my list anymore. I'm not saying there aren't any bugs, but I've reworked it to a point where the basic elements are doing what they should. This is a version that can be fixed, updated and upgraded without having to redo like half of it.

Nokta notes started out as a test project to try out Tauri. A simple idea: build a note editor with a clean UI that works with a database and has its own file format. It didn't take long for me to realise that I was building something I would actually use myself. A lot of cool ideas came up, but at the same time, even the basic version of today has a lot of little details. I made a concious decision to park all the cool ideas and focus on finishing a basic version.

This is what I'm proud of - or should I say: this was a total pain in the ass to build:

    Getting the application menu to reflect the app's status (like adding check marks and disabling menu items)
    Interacting safely with the database
    Deciding to completely change the text-editor (several times) before landing on Lexical, then making it behave how I want it.
    Actually doing all the little tweaks and optimizations I found along the way
    Fixing the search and replace functionality, search highlighting, the search UI, search keyword selection, fixing search bugs, search search search search...
    And this just in: Azure Trusted Signing!

I've been working on this app for a long time, and I think the foundation stands. Making it as solid as possible will be a goal for each upcoming version. With this first published version, I can finally start working on the new stuff that lives in my head for now.
v0.10.0 - Solid Foundations (AI Summary of the changelog)

A lot got cleaned up this cycle. Formatting bugs are gone: text colors, highlights, indentation, tabs in lists and code blocks — all behaving. Search and replace finally acts like a grown-up: highlights update correctly, clear when switching notes, and show informative messages.

UI polish got a big round of love too: the search panel has a close button, modal checkboxes aren’t the size of dinner plates anymore, error text is selectable, menu items enable and disable at the right times, and the app remebers scroll positions when switching betwee notes.

Big stability wins landed: corrupted or fake databases no longer blow up the app, deleting or restoring notes updates the UI instantly, reloading pulls from the database instead of the file (oops), and opening deleted notes correctly greys out actions.

Hydration, and lazy loading all came online smoothly to improve performance with large notes, with edge cases fixed along the way. Dragging notes into other notes is tighter, block quotes and code blocks look consistent, and paste-spam is blocked so users can’t fry the editor by accident.

In short: tons of formatting fixes, smarter search, cleaner UI, safer error handling, and a much more stable editor. The whole app just feels more solid now.
