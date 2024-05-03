# Testing

## Compatability

All pages have been tested for compatability in different browsers, including Google Chrome (default browser), Safari and Mozilla Firefox.

![Broswer Compatibility](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/Browser%20Compatability.png)

## Responsiveness

Home page responds well when tested on different device sizes. 

Note when increasing display size, the burger menu responds and branches out into inline menu in navbar, once into desktop view, the items in the menu show a line underneath when hovering over each one. When increasing display size, section elements also grow larger and flex-direction changes from column to row, with content displaying differently for each size, ensuring readability. Buttons also become active on desktop with hover function changing background and text colour for user experience.

![Home responsiveness](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/Home%20responsive.gif)

Seasonal Suggestions page also responds well, with the same elements changing as the displays grow larger and change flex-direction. Video displays well and plays in all sizes.

![Seasonal Suggestions responsiveness](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/Seasonal%20Suggestions%20responsive.gif)

Subscribe page also responds well, with increase in display size altering the flex-direction of radio buttons and input elements from column to row, also adjusting the spacing and alignment of all items as the display grows larger. Button becomes interactive with hover feature on desktop display.

![Subscribe responsiveness](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/Subscribe%20responsive.gif)

Response page also responds well, again, with increase in display size adjusting the layout of the section content. Button also becomes interactive with hover feature on desktop display.

![Response responsiveness](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/Response%20responsive.gif)

## Manual Testing



## Validator Testing

### HTML 

#### Home page

Initial errors reported:

![index validation errors](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/html%20index%20validation%20errors.png)

Fixes:

1: Removed second id from h1 (on all pages). Changed anchor tag from "top" to "logo" to target h1 still with 'top button'.

2: Removed controls command from iframe element.

3: Removed muted command from iframe element and added '&mute=1' to video source.

After re-validating code, page passed.

![HTML validation pass]()

#### Seasonal Suggestions page

Initial errors reported:

![seasonal suggestions validation errors](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/html%20seasonal-suggestions%20validation%20errors.png)

Fixes:

2: Removed controls command from iframe element.

3: Removed muted command from iframe element and added '&mute=1' to video source.

After re-validating code, page passed.

![HTML validation pass]()

#### Subscribe Page

Initial errors reported:

None, page passed HTML validation.

![]

#### Response Page

Initial errors reported:

None, page passed HTML validation.

### CSS

### Lighthouse Report / Performance

#### Home page

#### Seasonal Suggestions page

#### Subscribe Page

#### Response Page

## Bugs

### Solved Bugs

### Unsolved/Ongoing Bugs

## Mistakes

### Repository v1

