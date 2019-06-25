
----
Please respect the opensource Apache Version 2.0 License, and enjoy reading :)
----

# User story and modular docs 101
Open source training material on user stories and modular docs.
The repo has been tested downstream and will build using `CCTUIL`. Run the `CCTUIL` command in the root folder (that is, against the *master.adoc* file).

# Contribution guide

If you simply want to fix something small, fork the repo and create a PR against this repo.

If you want to add your own assembly, fork the repo and:

1) Make a copy of the `assembly-your-contribution` folder and use this as a basis for contributing.
2) Modify _your_ copy of the `assembly-your-contribution` folder and build it out in alignment with the existing repo structure.
3) When you are ready to locally test your work, add it to the `master.adoc`, for example:
----
//(3) Describes an *approach* that can be used when creating modular docs
include::./assembly-user-story-and-modular-docs-workflow/assembly-user-story-and-modular-docs-workflow.adoc[leveloffset=+1]

//(4) <Enter a one-liner that describes the purpose of your assembly>
include::./ ....................

//(5) ***TODO*** - add your contribution
include::./assembly-your-contribution/assembly-your-contribution.adoc[leveloffset=+1]
----
4) Create a username in the `upstream-resources/upstream-attributes.adoc` for example, `:jstaffor: jstaffor` and update _your_
new assembly so that the line `_Contribution made by:_ {user}` now displays _your_ username, for example, `_Contribution made by:_ {jstaffor}`. This is important for transparency and accountability purposes.

5) Test that the repo builds locally. `CCTUIL` is the recommended tool.

6) If the repo builds successfully, final create a PR and await a review :)

# Directory structure

----
master.adoc

  |____ assembly-combining-user-stories-and-modular-docs

    |____ assembly-combining-user-stories-and-modular-docs.adoc

    |____ concept-combining-user-stories-and-modular-docs.adoc

    |____ reference-user-story-and-modular-docs-example.adoc

    |____ procedure-user-story-and-modular-docs-example.adoc

  |____ assembly-user-story-and-modular-docs-101

    |____ assembly-user-story-and-modular-docs-101.adoc

    |____ concept-user-story-and-modular-docs.adoc

    |____ reference-user-story-principle.adoc

    |____ reference-modular-docs-principle.adoc

  |____ assembly-user-story-and-modular-docs-workflow

    |____ assembly-user-story-and-modular-docs-workflow.adoc

    |____ concept-combining-user-stories-and-modular-docs.adoc

    |____ analysis-user-story-and-modular-docs-workflow.adoc

    |____ planning-user-story-and-modular-docs-workflow.adoc

----
