# General
- [ ] The issue described in the ticket has been resolved.
- [ ] Any acceptance criteria listed in the ticket have been met.
- [ ] Additional tickets have been created for all TODOs and FIXMEs.
    - If you work on a team that uses TODOs and FIXMEs, they need to have a ticket before this code is sent for review. How else can you ensure the task is addressed? 
# New Variables
- [ ] . . . have good names.
    - A good name is concise and descriptive. Failing that, the next best name is long and descriptive. Unclear names waste valuable developer time and energy.
- [ ] . . . have the smallest possible scope.
    - Keep all code on a “need to know” basis. You can always increase the scope later if needed.
- [ ] . . . are declared/defined and initialised in the correct place within their function/class/module/file
# New Functions/Methods
- [ ] . . . have good names.
    - See note above for new variables.
- [ ] . . . have the smallest possible scope.
    - See note above for new variables.
- [ ] . . . are in the correct place within their class/module/file.
    - If a convention exists for the order in which the functions are listed in each class/module/file, follow it. This keeps the codebase organised, which makes it faster and easier to navigate. Some common conventions are:
        - alphabetical order
        - oldest to newest
        - separate sections for public vs. private functions
- [ ] . . . are unit-tested.
    - Not every function is unit-testable, but the ones that are should be unit-tested.
    - Will functions that are not unit-testable be covered by a different type of test? A UI test? An integration test?
# New Modules/Classes
- [ ] . . . have good names.
    - See note above for new variables.
- [ ] . . . have the smallest possible scope.
    - See note above for new variables.
- [ ] . . . are in the correct place within their file.
- [ ] . . . are tested.
# New Files
- [ ] . . . are appropriately named.
    - The name is fitting, spelt correctly, cased correctly, and follows any naming conventions already established in the codebase. 
    - Don’t make someone else create another PR later to rename your incorrectly named file. This is a massive waste of developer time, and file renames can make version control history more complicated to read and understand. This is an area where it pays off to get it right the first time.
- [ ] . . . are in the correct location in the correct directory.
    - Don’t make someone else create another PR later to move your file to the correct location. Files that aren’t in the correct place are more challenging to find and cause problems later on. Unnecessary file moves needlessly muddle version history.
# New Folders
- [ ] . . . are appropriately named.
    - See notes above for new files.
- [ ] . . . are in the correct location in the correct directory.
    - See note above for new files.
# Laser-focused
- [ ] There are no unnecessary whitespace changes.
    - Unnecessary white space changes clutter up your version history. They add useless commit history to that line of code and to that file. This makes everyone’s lives harder when things go wrong (which is the last thing you need when things go wrong!)
- [ ] Any refactors have been separated into their own PRs.
    - (If it can’t stand alone, it is not a refactor.)
- [ ] There are no unrelated code changes.
# Tests
- [ ] UI tests have been added for any new user interfaces.
- [ ] End-to-end tests have been added for any new features.
- [ ] Contract tests have been added for any new APIs.
- [ ] All tests have been run.
    - This means all tests for the entire codebase, not just the new tests.
# Localisation/Internationalisation/Translations
- [ ] All strings are localised.
    - Ideally, you have a script to check this, and CI runs that script.
- [ ] Translations (if available) have been added.
    - Ideally, you have a script to check this, and CI runs that script.
# Monitoring/Observability
- [ ] User analytics are being captured.
- [ ] Metrics are logged.
- [ ] Errors are logged.
- [ ] Alerts have been set up.
- [ ] Dashboards have been set up to display data when it starts coming in.
- [ ] A plan has been put in place for who will “own” these dashboards, i.e., whose job it is to monitor them, when and how often they will be checked, and how long they need to be monitored.
# Accessibility
- [ ] Text is provided for screen readers.
- [ ] _Checklist item regarding support for iOS's Dynamic Text coming soon_ 
# Security
- [ ] _Checklist items coming soon_
# Documentation
- [ ] Existing documentation has been updated (internal and external).
- [ ] New documentation has been written (internal and external).
# Due Diligence
- [ ] The code has been compiled and executed.
    - You may think this is obvious, but I cannot tell you the number of times I made a tiny change that I was 100% confident didn’t break anything and sent it off to review to find I was wrong.
- [ ] No new compile warnings or errors have been introduced to the codebase.
- [ ] All automated tools have been run.
    - Linters, static analysers, code formatters, code coverage, performance tests, etc.
    - Ideally, this is handled by CI.
- [ ] You have manually tested your work.
    - In other words, perform QA yourself.
- [ ] You have self-reviewed your code.
