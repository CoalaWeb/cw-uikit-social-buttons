## Table of Contents

1.  [Intro](#intro)
2.  [Quick Start](#qstart)
    -   [Requirements](#qstart-req)
    -   [Button Creation](#qstart-btn)
3.  [Extended Option](#options)
    -   [Button Size](#opt-size)
    -   [Button Icons](#opt-icons)
    -   [Button Text](#opt-text)
    -   [Button Count](#opt-count)
4.  [Current Networks](#networks)
5.  [Tested](#tested)
6.  [License](#license)
7.  [Issues?](#issues)

## <a name="intro"></a>Intro

> Are you using UIkit on its own or packaged with a template/theme/extension?
 
> Do you need a quick and easy way to get uniform social buttons on your site? 

By adding the `cw-uikit-social-buttons.css` file to your pages you can harness the power of UIkit and get great looking buttons in minutes.

![Figure-1](http://cdn.coalaweb.com/images/github/uikit/cw-uikit-social/button-examples.png "Figure-1"){.coalaweb-docs}

## <a name="qstart"></a>Quick Start

### <a name="qstart-req"></a>Requirements

**UIkit:** The first thing you need to do is to make sure you have UIkit loading on your site. To check right click your page and select **View Page Source** then have a look in the head of the page for a reference to UIkit. *\[Figure 2\]*

![Figure-2](http://cdn.coalaweb.com/images/github/uikit/cw-uikit-social/include-uikit.png "Figure-2"){.coalaweb-docs}

>  Note: If you are using a YooTheme template or any other YooTheme extension then you will already have it loading.

**CW UIkit Social Buttons:** Next include the `cw-uikit-social-buttons.css` on your page. You can check if its loaded the same way as above. *\[Figure 3\]*

![Figure-3](http://cdn.coalaweb.com/images/github/uikit/cw-uikit-social/include-social-css.png "Figure-3"){.coalaweb-docs}

**jQuery:** Lastly make sure to include the jQuery on your page. You can check if its loaded the same way as above. *\[Figure 4\]*

![Figure-4](http://cdn.coalaweb.com/images/github/uikit/cw-uikit-social/include-jquery.png "Figure-4"){.coalaweb-docs}

> Note: If you have files listed but they don't appear to be working make sure the files are reachable by clicking on the link when viewing the page source. If it opens then its reachable.

### <a name="qstart-btn"></a>Button Creation

Now lets add some buttons, I prefer to have the buttons in a list but thats up to you. Below we have a few outer containers to help with the layout and then inside that we have our list container and one button in its default state.

```html
<div class="uk-container uk-margin-top uk-margin-bottom">
    <div class="uk-grid" data-uk-grid-margin="">
        <div class="uk-width-1-1 uk-text-left">
            <ul class="cw-social-container">
                <li class="">
                    <a href="#" class="uk-button uk-contrast cw-social cw-twitter">Twitter</a>
                </li>
            </ul>
        </div>
    </div>
</div>
```

The minimum attributes that you will need to include with your buttons are:

- `uk-button`
- `uk-contrast`
- `cw-social`
- `cw-twitter`

> Note: You can choose which social network based on the currently supported [Networks List](#networks)

### <a name="options"></a>Extended Options

You have several options to extend the functionality of the buttons such as **size**, **icon**, **text** and **count**.

#### <a name="opt-size"></a>Button Sizes

The buttons can be displayed in a variety of sizes which included:

**Default:** 
- Link class = 
- Button class = 
- Icon class = 

**Small:** 
- Link class = `cw-small`
- Button class = `cw-small`
- Icon class = `uk-icon-small`

**Medium:** 
- Link class = `cw-medium`
- Button class = `cw-medium`
- Icon class = `uk-icon-medium`

**Large:** 
- Link class = `cw-large` 
- Button class = `cw-large`
- Icon class = `uk-icon-large`

```html
<div class="uk-button-group">
    <a href="#" class="uk-button uk-contrast cw-social cw-small cw-google-plus">
        <i class="uk-icon-google-plus uk-icon-small"></i> Google</a>
    <button class="uk-button cw-share-count cw-small">313</button>
</div>
```

#### <a name="opt-icon"></a>Button Icon

Then if you want to add an icon use an `<i>` tag with a class using the social network you want to display.

`<i class="uk-icon-twitter"></i>` 

> Note: You can choose which social network based on the currently supported [Networks List](#networks)

> Note: The icon will also have to match your **Link/Button** size:

**Default:**
- Icon Class = 

**Small:**
- Icon Class = `uk-icon-small`
 
**Medium:**
- Icon Class = `uk-icon-medium`
 
**Large:**
- Icon Class = `uk-icon-large`

```html
<div class="uk-button-group">
    <a href="#" class="uk-button uk-contrast cw-social cw-small cw-google-plus">
        <i class="uk-icon-google-plus uk-icon-small"></i> Google</a>
    <button class="uk-button cw-share-count cw-small">313</button>
</div>
```

#### <a name="opt-text"></a>Button Text

The buttons can be displayed with or without text.

**Text:** 
- Icon class = 

```html
<a href="#" class="uk-button uk-contrast cw-social cw-twitter">
    <i class="uk-icon-twitter"></i> Twitter</a>
```

> Note: Make sure to leave a space after the icon.

**No Text:** 
- Icon class = `cw-no-text`

```html
<a href="#" class="uk-button uk-contrast cw-social cw-twitter">
    <i class="uk-icon-twitter cw-no-text"></i></a>
```

#### <a name="opt-count"></a>Button Count

If you want to display a count just add a surrounding `<div>` element with the class attribute `uk-button-group` and a `<button>` element with the class attribute of `uk-button cw-share-count`.

```html
<div class="uk-button-group">
    <a href="#" class="uk-button uk-contrast cw-social cw-twitter">
        <i class="uk-icon-twitter"></i> Twitter</a>
    <button class="uk-button cw-share-count">313</button>
</div>
</div>
```

> Note: The count will also have to match your **Link/Icon** size:

**Default:**
- Button Class = 

**Small:**
- Button Class = `cw-small`
 
**Medium:**
- Button Class = `cw-medium`
 
**Large:**
- Button Class = `cw-large`

```html
<div class="uk-button-group">
    <a href="#" class="uk-button uk-contrast cw-social cw-small cw-google-plus">
        <i class="uk-icon-google-plus uk-icon-small"></i> Google</a>
    <button class="uk-button cw-share-count cw-small">313</button>
</div>
```

## <a name="networks"></a>Current Networks

The currently support social networks are:

**Facbook:**
- Link Class = `cw-facebook`
- Button Class = `cw-facebook`
- Icon Class = `uk-icon-facebook`

**Google:**
- Link Class = `cw-google-plus`
- Button Class = `cw-google-plus`
- Icon Class = `uk-icon-google-plus` or `uk-icon-google`

**Twitter:**
- Link Class = `cw-twitter`
- Button Class = `cw-twitter`
- Icon Class = `uk-icon-twitter`

**Linkedin:**
- Link Class = `cw-linkedin`
- Button Class = `cw-linkedin`
- Icon Class = `uk-icon-linkedin`

**Reddit:**
- Link Class = `cw-reddit`
- Button Class = `cw-reddit`
- Icon Class = `uk-icon-reddit`

**Stumbleupon:**
- Link Class = `cw-stumbleupon`
- Button Class = `cw-stumbleupon`
- Icon Class = `uk-icon-stumbleupon`

**Digg:**
- Link Class = `cw-digg`
- Button Class = `cw-digg`
- Icon Class = `uk-icon-digg`

**Pinterest:**
- Link Class = `cw-pinterest`
- Button Class = `cw-pinterest`
- Icon Class = `uk-icon-pinterest`

**Mail:**
- Link Class = `cw-mail`
- Button Class = `cw-mail`
- Icon Class = `uk-icon-envelope`

**Github:**
- Link Class = `cw-github`
- Button Class = `cw-github`
- Icon Class = `uk-icon-github`

**Flickr:**
- Link Class = `cw-flickr`
- Button Class = `cw-flickr`
- Icon Class = `uk-icon-flickr`

## <a name="tested"></a>Tested

#### UIkit
- **UIkit:** 2.24.3

#### jQuery
- **jQuery:** 2.1.4

#### Browsers
- **Firefox:** 41.0.1
- **Chrome:** 45.0.2454.101
- **Opera:** 32.0.1948.69
- **IE:** 11.0.9600.18015
- **Safari:** 9.0.2

## <a name="license"></a>License

Dual licensed under the [MIT](http://www.opensource.org/licenses/mit-license.php) and [GPL](http://www.gnu.org/licenses/gpl.html) licenses:

## <a name="issues"></a>Issues

Do you have an issue? Found a bug? Want to request a new feature? Then create a new issue [here](https://github.com/CoalaWeb/cw-uikit-social-buttons/issues).
