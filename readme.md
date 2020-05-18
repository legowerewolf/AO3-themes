# AO3 Work Skins

Easy-to-use skins for works on Archive of Our Own.

Have an idea, but don't know what to do?
[Make an issue](https://github.com/legowerewolf/AO3-themes/issues/new) and I'll work with you to
bring your idea to fruition.

## Skins

Each skin below is built using the modular components listed. Descriptions of each component and how
to use it are [here](https://github.com/legowerewolf/AO3-themes/tree/master/src/components).

-   Generic theme: [demo](https://archiveofourown.org/works/16349828) {images, skin-warning,
    book-paragraph, texting} (generic.css)

## Installation

1. Log in to AO3, go [here](https://archiveofourown.org/skins?skin_type=WorkSkin), and click "Create
   Work Skin." Or, click [here](https://archiveofourown.org/skins/new?skin_type=WorkSkin).
2. Fill out the form. Name, description, etc.
3. Copy the contents of the built skin (from the
   [latest release](https://github.com/legowerewolf/AO3-themes/releases/latest)) to the big empty
   CSS box.
    > Tip: If you only want some of the features, look for the headings enclosed by `/*` and `*/` -
    > they indicate what the following styles do.
4. Hit "Submit" at the bottom.

## Usage

When drafting a work, select the skin you created above from the drop-down menu in the
"Associations" box, under the collections, gifting, and series settings. Also, please add a link
back to here in the notes for other people to see! It'll help other authors discover this skin.

## Tips

If you don't need to do anything weird with formatting? Write your stories in Word or Google Docs
and copy them into the rich text editor. That'll handle any of the common formatting (like italics
or bolding) and make sure you're generating valid markup to render.

On the flip side, if you do need to do something odd, you're gonna have to code it manually. I
recommend writing up as much of your story in a standard document editor like Word or Docs and
leaving a little note for where you need to insert non-standard stuff. Copy and paste the whole
thing into the rich text editor, then find and replace that note with your actual code.

If you're really having issues, let me know on one of my platforms [here](https://legowerewolf.net)
or through the issue form above and I'll do my very best to help you.

### Sanitization

Archive of Our Own runs your input through a _sanitizer_ to make sure it's safe to share with the
world. It enforces a number of rules, which can be found
[here.](https://archiveofourown.org/help/html-help.html)

Here are some quirks I've noticed:

-   The only root elements allowed are paragraphs (`<p>`) and content divisions with a class
    attribute (`<div class="somename">`). Everything else will be wrapped in a paragraph.

### Composition

You're writing a story, not building a website. Regardless, when drafting in HTML, you should use an
actual code editor. [Visual Studio Code](https://code.visualstudio.com/) is lightweight and easy to
use.

-   Image `<img>` tags should go inside a content division.

    This will work, but not quite right. It'll get wrapped in a paragraph tag.

    ```html
    <img src="..." />
    ```

    This will work better:

    ```html
    <div class="_">
        <img src="..." />
    </div>
    ```

### Testing

I've included a `demo.html` file that includes the generic stylesheet and adds styles for validating
content. Compose between the `<!-- comments -->`, and open it in your browser to check. If it comes
up surrounded in a red box, the sanitizer might get mad at you.
