# AO3 Work Skins

[![ko-fi](https://www.ko-fi.com/img/donate_sm.png)](https://ko-fi.com/O4O6QKLP)

Easy-to-use skins for works on Archive of Our Own. All skins below are built using the modular components listed [here](https://github.com/legowerewolf/AO3-themes/tree/master/src/components).

Skins

-   Generic theme: [demo](https://archiveofourown.org/works/16349828), [source](https://raw.githubusercontent.com/legowerewolf/AO3-themes/master/build/generic.css) {images, skin-warning, paragraph, texting}

## Installation

1. Log in to AO3, go [here](https://archiveofourown.org/skins?skin_type=WorkSkin), and click "Create Work Skin." Or, click [here](https://archiveofourown.org/skins/new?skin_type=WorkSkin).
2. Fill out the form. Name, description, etc.
3. Copy the contents of the built skin (the source link in the list above) to the big empty CSS box.
    > Tip: If you only want some of the features, look for the headings enclosed by `/*` and `*/` - they indicate what the following styles do.
4. Hit "Submit" at the bottom.

## Usage

When drafting a work, select the skin you created above from the drop-down menu in the "Associations" box, under the collections, gifting, and series settings. Also, please add a link back to here for other people to see! It'll help other authors discover this skin.

## Tips

-   Any HTML not in a `<p>` or `<div>` tag will get wrapped in a `<p>` tag by the Archive's HTML sanitizer. Images and other elements should get wrapped in a `<div>` for the formatting to apply properly.
