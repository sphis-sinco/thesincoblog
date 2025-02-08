---
title: "Learnings: Haxeflixel project XML"
datePublished: Sat Feb 08 2025 21:03:23 GMT+0000 (Coordinated Universal Time)
cuid: cm6womynl000m08jybzt8fvb5
slug: learnings-haxeflixel-project-xml
tags: learning, learnings, sinco

---

# The start

Can you tell me what this XML code does?

```xml
<set name="buildOrTest" if="${project.command == build} || ${project.command == test}" />
<echo value="Building for ${project.target} on a ${project.host} machine" if="buildOrTest" />

<echo value="${meta.title} v${meta.version}" />
```

No? Well, I can tell you.

That first line sets the value of `buildOrTest` to if the project is being compiled with `lime test` or `lime build`.

The second line executes only if `buildOrTest` is true and prints to the console what platform you're compiling to and what machine you're compiling with.

For example: “`Building for mobile on a windows machine`”.

Now the third line is unrelated and just prints to the console the project title and version.

“`Sinco and Portilizen v0.0.3`“ for example.

Today I decided to stream some development of Sinco and Portilizen and I decided to do backlog and quality of life stuff.

I moved folders to a central sap folder so that if I am overwriting files then I won’t confuse that folder for just a random folder name. The chances of that are unlikely but I’m just inspired by Funkin a lot so leave me alone.

And then I moved from traces from Initialization to the project.xml using things I didn’t even know existed for project XML files.

Alright let’s get started

# Elements I’ve learned

## Echo

Echo is pretty simple, it’s like trace but it doesn’t show what file it comes from. It’s the echo command in your terminal.

## Set

This is setting a variable but in XML. For example:

```xml
<set name="debug" if="DEBUG_BUILD"/>
```

That line of code sets `debug` to true if you are compiling with the `DEBUG_BUILD` compiler condition

## Define

This is basically **Set** but for compiler conditions

## Section

It’s basically like a function. If it has an if argument set then it is dependent on a condition. For example:

```xml
<section>
<section/>
```

That will run always.

```xml
<section if="DEBUG_BUILD">
<section/>
```

That will run if compiled with the `DEBUG_BUILD` Compiler Condition

## Error

It’s **Set** but with this cool little `Error:` text in the front and it stops the game from compiling.

# Final thoughts

Project.xml is noice.

If you don’t like it then you probably should look at the [docs](https://lime.openfl.org/docs/project-files/xml-format/).

You don’t have to use trace to figure out what compiler flags are being used thanks to the docs so uh, yeah.

Ok time for the article quote:

“Start with a mess and clean it up later.“