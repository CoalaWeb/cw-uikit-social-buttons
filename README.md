## Table of Contents

1.  [Intro](#intro)
2.  [Quick Start](#qstart)
3.  [Extended Option](#options)
    -   [Button Sizes](#opt-size)
    -   [Button Text](#opt-text)
    -   [Button Count](#opt-count)
4.  [Tested](#tested)
5.  [License](#license)
6.  [Issues?](#issues)

## <a name="intro"></a>Intro

> Are you using UIkit on its own or are you using a template/theme or extension that has come packaged with it?
 
> Do you need a quick and easy way to get uniform social buttons on your site? 

Then you have come to right place all you have to do is included the **cw-uikit-social-buttons.css** file to harness the power of UIkit and get great looking buttons in minutes.

![Figure-1](http://cdn.coalaweb.com/images/github/uikit/cw-uikit-social/button-examples.png "Figure-1")

## <a name="qstart"></a>Quick Start

The first thing you need to do is to make sure you have **UIkit** loading on your site. To check right click your page and select **View Page Source** then have a look in the head of the page for a reference to UIkit. *\[Figure 2\]*

![Figure-2](http://cdn.coalaweb.com/images/github/uikit/cw-uikit-social/include-uikit.png "Figure-2")

>  Note: If you are using a YooTheme template or any other YooTheme extension then you will already have it loading.

Next include the **cw-uikit-social-buttons.css** on your page. You can check if its loaded the same way as above. *\[Figure 3\]*

![Figure-3](http://cdn.coalaweb.com/images/github/uikit/cw-uikit-social/include-social-css.png "Figure-3")

Lastly make sure to include the **jQuery** on your page. You can check if its loaded the same way as above. *\[Figure 4\]*

![Figure-4](http://cdn.coalaweb.com/images/github/uikit/cw-uikit-social/include-jquery.png "Figure-4")

> Note: If you have files listed but they don't appear to be working make sure the files are reachable by clicking on the link when viewing the page source. If it opens then its reachable.

Now lets add some buttons, I prefer to have the buttons in a list so they flow nicely on different page widths. Below we have some outer containers to help with the layout and then inside that we have our list container and one button in its default state with an icon.

```html
<div class="uk-container uk-margin-top uk-margin-bottom">
    <div class="uk-grid" data-uk-grid-margin="">
        <div class="uk-width-1-1 uk-text-left">
            <ul class="cw-social-container">
                <li class="">
                    <a href="#" class="uk-button uk-contrast cw-social cw-twitter">
                        <i class="uk-icon-twitter"></i> Twitter</a>
                </li>
            </ul>
        </div>
    </div>
</div>
```

The important thing is to create your link and give it a class of at least:

- uk-button
- uk-contrast
- cw-social
- cw-twitter (you can choose based on the list below)

Then if you want to add an icon use an `<i>` tag with the class of:

- uk-icon-twitter (you can choose based on the list below)

The currently support social networks are:

- Facebook
- Google
- Twitter
- Linkedin
- Reddit
- Stumbleupon
- Reddit
- Digg
- Pinterest
- Mail

### <a name="options"></a>Extended Options

You gave several options to extend the functionality of the buttons such as size, text and count.

#### <a name="opt-size"></a>Button Sizes

The buttons can be displayed in a variety of sizes which included:

**Default:** 
- No link class added
- No Icon class added

**Small:** 
- Link class = cw-small
- Icon class = uk-icon-small

**Medium:** 
- Link class = cw-medium
- Icon class = uk-icon-medium

**Large:** 
- Link class = cw-large 
- Icon class = uk-icon-large

```html
<a href="#" class="uk-button uk-contrast cw-social cw-small cw-twitter">
    <i class="uk-icon-twitter uk-icon-small"></i></a>
```

#### <a name="opt-text"></a>Button Text

The buttons can be displayed with or without text.

**Text:** 
- No link class added just make sure to leave a space after the icon.

```html
<a href="#" class="uk-button uk-contrast cw-social cw-twitter">
    <i class="uk-icon-twitter"></i> Twitter</a>
```

**No Text:** 
- Icon class = cw-no-text

```html
<a href="#" class="uk-button uk-contrast cw-social cw-twitter">
    <i class="uk-icon-twitter cw-no-text"></i> Twitter</a>
```

#### <a name="opt-count"></a>Button Count

You can also display a count for each of the buttons by adding a simple `<span>` element.

```html
<a href="#" class="uk-button uk-contrast cw-social cw-twitter">
    <i class="uk-icon-twitter"></i> Twitter</a><span class="cw-share-count ">313</span>
```

The count will also have to match your button size:

**Default:**
- No span class added
**Small:**
- Span Class = cw-small 
**Medium:**
- Span Class = cw-medium 
**Large:**
- Span Class = cw-large

```html
<a href="#" class="uk-button uk-contrast cw-social cw-small cw-twitter">
    <i class="uk-icon-twitter uk-icon-small"></i> Twitter</a><span class="cw-share-count cw-small">313</span> 
```

## <a name="tested"></a>Tested

#### UIkit
-   **UIkit:** 2.24.2

#### jQuery
-   **jQuery:** 1.11.3

#### Browsers
-   **Firefox:** 41.0.1
-   **Chrome:** 45.0.2454.101
-   **Opera:** 32.0.1948.69
-   **IE:** 11.0.9600.18015

## <a name="license"></a>License

Dual licensed under the [MIT](http://www.opensource.org/licenses/mit-license.php) and [GPL](http://www.gnu.org/licenses/gpl.html) licenses:

## <a name="issues"></a>Issues

Do you have an issue? Found a bug? Want to request a new feature? Then create a new issue [here](https://github.com/CoalaWeb/cw-uikit-social-buttons/issues).
