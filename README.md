// Copy this Template.
// Describe the title of your article by replacing "How-to Template" with the page name you want to publish to.
= How-to template
include::../adoc-parameters.txt[]
// Article variables (delete the `// comments` and add in the values)
:description: #Summarise what this how-to article is about in a sentence or two. What you put here is reused in the Overview section and included in HTML description tags.#
:keywords: #These are comma-separated tags, similar to labels#

== Overview

{description}

== Before you start
// Delete this section if your readers can dive straight into the lesson without requiring any pre-requisite knowledge.
Make sure you meet the following pre-requisites before starting the how-to steps:

* Pre-requisite one
* Pre-requisite two
* etc

== Step-by-step guide

// If your how-to is simple (it doesn't contain screenshots or code samples) you can use an ordered list for your procedure. Otherwise use the step table.

[cols="a,a,a" options="header,autowidth"]
|===
|Step
|Task
|Screenshot or example

|1
|Lead-in sentence for an ordered list:

. Step 1
. Step 2
. Step 3

|image::https://upload.wikimedia.org/wikipedia/commons/3/35/Tux.svg[Tux,250,350]

|2
|Run the `apt` command to install the Asciidoctor package and check the version.
|
[source]
----
$ sudo apt install asciidoctor

$ asciidoctor --version
Asciidoctor 1.5.6.2 [https://asciidoctor.org]
----

|===
