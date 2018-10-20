# AO3 General Work Skin

Easy-to-use skin for works on Archive of Our Own. 
This skin adds:

* Image display fixes - no more overflow that's hard for mobile users to see!
* Easy-to-use texting formatting - with colors and labels for all your texting and group-chat fic needs.
* Warnings about the usage of work skins. If users can't see the skin, it doesn't do them any good.

## Installation

1. Log in to AO3, go [here](https://archiveofourown.org/skins?skin_type=WorkSkin), and click "Create Work Skin." Or, click [here](https://archiveofourown.org/skins/new?skin_type=WorkSkin).
2. Fill out the form. Name, description, etc.
3. Copy the contents of [this page](https://raw.githubusercontent.com/legowerewolf/AO3-themes/master/main.css) to the big empty CSS box.
4. Hit "Submit" at the bottom.

## Usage

When drafting a work, select the skin you created above from the drop-down menu in the "Associations" box, under the collections, gifting, and series settings.

### Images

Add images just as you normally would. The CSS will center the image and scale it to fit within the width of the user's device/browser window.

### Texting

This takes a bit more work. You're gonna want the HTML editor for this. 

1. Create a `div` with the `texting-container` class.
    ```html
    <div class="texting-container">

    </div>
    ```
2. Add a `div` inside of it, with the side of the screen you want the messages inside to be on and their color as classes. For sides, you can use `right` and `left`, and for colors you can use `red`, `blue`, `teal`, `green`, `yellow`, and `orange`.
    ```html
    <div class="texting-container">
        <div class="left red">

        </div>
    </div>
    ```
3. Optionally, you can add the person's name inside a paragraph element with the class `name`.
    ```html
    <div class="texting-container">
        <div class="left red">
            <p class="name">Edgelord</p>
        </div>
    </div>
    ```
4. Finally, you add messages. 
    ```html
    <div class="texting-container">
        <div class="left red">
            <p class="name">Edgelord</p>
            <p>Hi, I'm an edgy edgelord.</p>
        </div>
    </div>
    ```

For each change in speaker, you'll have to repeat steps 2-4. No way around it. Sorry. This is already much better than how it worked before I did a bunch of fixing. No more classes for top, middle, and bottom messages to get the bubbling looking right.

### Skin Usage Warning

This one is simple. You just want to include any element with the class `skin-warning`. Any element with that class will be hidden *if* work skins are enabled. I recommend something fairly simple, like below. Feel free to copy and paste this into your code.

```html
<p class="skin-warning"><b>A/N:</b> This work relies on a skin to make it look better. Enable the skin by clicking here: <a href="?style=creator">[Enable work skin]</a></p>
```

It'll look something like this: 

**A/N:** This work relies on a skin to make it look better. Enable the skin by clicking here: [[Enable work skin]](?style=creator).
