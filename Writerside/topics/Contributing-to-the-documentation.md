# Contributing to the documentation

<primary-label ref="stable"/>
<secondary-label ref="beta"/>

This documentation project uses Writerside.
If you want to edit it, you can click the <control>Edit page</control> button.

![Edit page](edit-page.png)

Then, you will be taken to GitHub where you can edit the page.
Once you are done, click <control>Commit Changes</control> and create a pull request.
<format color="BlueViolet">However, if possible please talk with us on
    <format color="DarkOrange">
        <a href="https://discord.com/invite/DrfX6286kF">discord</a>
    </format>
    or create a new
    <format color="DarkOrange">
        <a href="https://github.com/Chillax-ORG/chillaxdocs/issues/new">GitHub Issue</a>
    </format>
    beforehand
</format>.

## About Writerside

The Writerside documentation can be found
at [Writerside | JetBrains Marketplace](https://www.jetbrains.com/help/writerside/discover-writerside.html).

### Writerside syntax overview

Writerside syntax is based on Markdown, but with some extra features.

* Display keyboard shortcuts:

<!-- ```markdown -->

```
<shortcut>Ctrl + \\</shortcut>
```

results in <shortcut>Ctrl + \\</shortcut>

* Display menu selections:

<!-- ```markdown -->

```
<ui-path>File | New | CSS File</ui-path>
```

results in <ui-path>File | New | CSS File</ui-path>

* Reference elements like [headings on the same page](#writerside-syntax-overview):

<!-- ```markdown -->

```
[Refer to](#my-heading)

## My Heading
```

* Reference [other pages](Contributing-to-the-source-code.md):

<!-- ```markdown -->

```
[Other page](Contributing-to-the-source-code.md)
```

* To include images/gifs, put them in the `images` directory, possibly in a subdirectory, and use

<!-- ```markdown -->

```
![My Image](my-image.png)
```
