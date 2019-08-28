# AO3 Work Skins

[![ko-fi](https://www.ko-fi.com/img/donate_sm.png)](https://ko-fi.com/O4O6QKLP)

Easy-to-use skins for works on Archive of Our Own.

Have an idea, but don't know what to do? [Make an issue](https://github.com/legowerewolf/AO3-themes/issues/new) and I'll work with you to bring your idea to fruition.

## Skins

Each skin below is built using the modular components listed. Descriptions of each component and how to use it are [here](https://github.com/legowerewolf/AO3-themes/tree/master/src/components).

-   Generic theme: [demo](https://archiveofourown.org/works/16349828) {images, skin-warning, paragraph, texting}

## Installation

1. Log in to AO3, go [here](https://archiveofourown.org/skins?skin_type=WorkSkin), and click "Create Work Skin." Or, click [here](https://archiveofourown.org/skins/new?skin_type=WorkSkin).
2. Fill out the form. Name, description, etc.
3. Copy the contents of the built skin (from the [latest release](https://github.com/legowerewolf/AO3-themes/releases/latest)) to the big empty CSS box.
    > Tip: If you only want some of the features, look for the headings enclosed by `/*` and `*/` - they indicate what the following styles do.
4. Hit "Submit" at the bottom.

## Usage

When drafting a work, select the skin you created above from the drop-down menu in the "Associations" box, under the collections, gifting, and series settings. Also, please add a link back to here for other people to see! It'll help other authors discover this skin.

## Tips

### Sanitization

Archive of Our Own runs your input through a _sanitizer_ to make sure it's safe to share with the world. It enforces a number of rules, which can be found [here.](https://archiveofourown.org/help/html-help.html)

Here are some quirks I've noticed:

-   The only root elements allowed are paragraphs (`<p>`) and content divisions with a class attribute (`<div class="somename">`). Everything else will be wrapped in a paragraph.

### Composition

You're writing a story, not building a website. Regardless, when drafting in HTML, you should use an actual code editor. [Visual Studio Code](https://code.visualstudio.com/) is lightweight and easy to use.

-   Image `<img>` tags should go inside an otherwise-empty paragraph tag.
