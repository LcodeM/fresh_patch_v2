# Testing

## Compatability

All pages have been tested for compatability in different browsers, including Google Chrome (default browser), Safari and Mozilla Firefox.

![Broswer Compatibility](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/broswer_compatability.png)

## Responsiveness

Home page responds well when tested on different device sizes. 

Note when increasing display size, the burger menu responds and branches out into inline menu in navbar, once into desktop view, the items in the menu show a line underneath when hovering over each one. When increasing display size, section elements also grow larger and flex-direction changes from column to row, with content displaying differently for each size, ensuring readability. Buttons also become active on desktop with hover function changing background and text colour for user experience.

![Home responsiveness](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/home_responsivity.gif)

Seasonal Suggestions page also responds well, with the same elements changing as the displays grow larger and change flex-direction. Video displays well and plays in all sizes.

![Seasonal Suggestions responsiveness](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/seasonal_suggestions_responsive.gif)

Subscribe page also responds well, with increase in display size altering the flex-direction of radio buttons and input elements from column to row, also adjusting the spacing and alignment of all items as the display grows larger. Button becomes interactive with hover feature on desktop display.

![Subscribe responsiveness](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/subscribe_responsive.gif)

Response page also responds well, again, with increase in display size adjusting the layout of the section content. Button also becomes interactive with hover feature on desktop display.

![Response responsiveness](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/response_responsive.gif)

## Manual Testing



## Validator Testing

### HTML 

#### Home page

Initial errors reported:

![index validation errors](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/html_index_validation_errors.png)

Fixes:

1: Removed second id from h1 (on all pages). Changed anchor tag from "top" to "logo" to target h1 still with 'top button'.

2: Removed controls command from iframe element.

3: Removed muted command from iframe element and added '&mute=1' to video source.

After re-validating code, page passed.

![HTML validation pass](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/validation_pass.png)

#### Seasonal Suggestions page

Initial errors reported:

![seasonal suggestions validation errors](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/html_seasonal_suggestions_validation_errors.png)

Fixes:

1: Removed controls command from iframe element.

2: Removed muted command from iframe element and added '&mute=1' to video source.

After re-validating code, page passed.

![HTML validation pass](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/validation_pass.png)

#### Subscribe Page

Initial errors reported:

None, page passed HTML validation.

![HTML validation pass](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/validation_pass.png)

#### Response Page

Initial errors reported:

None, page passed HTML validation.

![HTML validation pass](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/validation_pass.png)

### CSS

Initial errors reported:

None, css passed validation.

![CSS validation pass](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/css_validator_pass.png)

### Lighthouse Report / Performance

#### Home page

index.html (Home) page is not performing well upon testing with lighthouse, as it contains an embedded Youtube video which is causing performance issues. However, I feel that the instructional video is paramount to the user as it provides good information and content to the 'Today's Top Tip' section. In future developments, one fix for this would be to use 'lazy loading' to the iframe source code, where videos are necessary.

Another fix for performance in future developments would be to use different image file types to optimize them for web use, instead of PNG. 

Mobile:
![index performance mobile](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/index_lighthouse_score_mobile.png)

Desktop:
![index performance desktop](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/index_lighthouse_score_desktop.png)

#### Seasonal Suggestions page

seasonal-suggestions.html (Seasonal Suggestions) page is not performing well upon testing with lighthouse, as it contains an embedded Youtube video which is causing performance issues. However, I feel that the instructional video is paramount to the user as it provides good information and content to the 'Today's Top Tip' section. In future developments, one fix for this would be to use 'lazy loading' to the iframe source code, where videos are necessary.

Another fix for performance in future developments would be to use different image file types to optimize them for web use, instead of PNG.

The same performance issues are being 
Mobile:
![seasonal suggestions performance mobile](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/seasonal_suggestions_lighthouse_score_mobile.png)

Desktop:
![seasonal suggestions performance desktop](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/seasonal_suggestions_lighthouse_score_desktop.png)

#### Subscribe Page

There are little to no performance issues with subscribe.html (Join) page.

Mobile:
![subscribe performance mobile](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/subscribe_lighthouse_score_mobile.png)

Desktop:
![subscribe performance desktop](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/subscribe_lighthouse_score_desktop.png)

#### Response Page

There are little to no performance issues with response.html (Response) page.

Mobile:
![response performance mobile](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/response_lighthouse_score_mobile.png)

Desktop:
![response performance desktop](https://github.com/LcodeM/fresh_patch_v2/blob/main/documentation/response_lighthouse_score_desktop.png)

## Bugs

### Solved Bugs

1: Didn’t know how to resize my image for mobile. What did I do? Used google, found Stack Overflow and DigitalOcean for support and reduced pixel size to even height and width (300px).

2: Didn’t know how to create a link to another internal page with a button. What did I do? Googled and found w3schools tutorial and used an element inside button to link to subscribe.html

3: Forgot how to fix the navigation bar and push content below the header. Used CI lessons and Love running code examples to find the size of the header, and increase the margin top for main content to a larger size. 

4: Confused as to how to push margins using different measurements. Found margin support on Sitepoint which explained rem/em sizing. Then realised I could just adjust the width to 100% for responsively on desktop. 

5: Footer was being pushed out to the top right of the page. Asked my classmates for support. Issue was with body styles, needed to add: flex-direction:column

6: Header began to drop to centre of page. Removed justify-content: centre from media query for small and large laptop screens body section.

7: Menu list and bars icon not displaying on mobile pages ‘seasonal-suggestions.html’ and ‘response.html’ . Issue was resolved by copying code from nav, footer and script sections from index.html to all other pages.

8: Duplicate menu items showing on  ‘Subscribe’ page in desktop view. Removed duplicate nav section from html on subscribe page and made correct link active.

9: ‘Today’s Top Tip’ section was not displaying padding above and below due to specificity rule breach in css targeting id above general style rule. 

10: text-decoration and colour not being applied to all buttons. Solution was to target the ‘a’ element text NOT the button styles.

11: a element not passing validation as a child/descendent of button. Changed html code to form element with a button, keeping styling and destination consistent.

12: image resolution making load times slower. Reduced all image resolution to 400x600px or 600x400px (depending on orientation).

13: “controls mute” not working on YouTube video. Stack overflow troubleshoot provided solution via previously solved issue, using ‘&mute=1’ code to source hyperlink. And resizing YouTube image window height & responsiveness: https://stackoverflow.com/questions/43011931/resize-embedded-video-links-html

14: Added ‘top’ button to index.html and seasonal-suggestions.html pages to enable users to quickly access the top of the page. Source: https://stackoverflow.com/questions/68627683/scroll-up-button-without-javascript

15: When opening on public server, h1 was showing black. Created style rule for h1 to make green, as this is the only h1 heading across all pages.

16: Was using % values to try and create a border-radius for all sections. Fixed this by using px instead.

17: Validator not accepting ‘controls’ or ‘muted’ in iframe. Added &mute=1 to source, removed controls command. 

18: html validator not accepting id=“logo top” in h1 - fixed by removing second “top” id (as not allowed 2 ids in an element) and replaced the anchor tag with “logo”.

### Unsolved/Ongoing Bugs

alt-text not displaying properly because of border-radius on circle images. Tried multiple troubleshooting solutions as per below links, but no success.

[psuedo classes](https://www.dev-diaries.com/social-posts/style-broken-images/) (for pseudo classes)
[fixing broken images](https://javascript.plainenglish.io/how-to-style-broken-images-using-css-b238c907c8af) (fixing broken images)
[onerror](https://www.w3schools.com/tags/ev_onerror.asp#:~:text=Definition%20and%20Usage,a%20document%20or%20an%20image) and [onerror](https://www.w3schools.com/jsref/event_onerror.asp) (onerror attribute)
[pseudo class list](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes) (List of pseudo-classes)

## Mistakes

### Repository v1

On Wednesday May 1st 2024, after completing all of the main content and CSS styling for the website, I encountered a 'head detached' error in my terminal. After seeking advice from my mentor, troubleshooting and trying to find the cause of the problem, it was determined that it would be easier and faster to create a new repository for my site, and simply migrate the code for all pages and CSS. 

After doing this, I also exported my git commits from version 1 of the website in order to maintain a full git log of the sites creation, which can be found [here](https://github.com/LcodeM/fresh_patch_v2/blob/main/V1LOG.md)

Note that all commits in the previous log from version 1 were also done in past tense and began with a lowercase letter. Upon recreation of my website in version 2, I was reminded to log git commits in present tense beginning with an uppercase letter, which I have tried my best to adhere to going forward.

Though this mistake was coslty in regard to time and energy spent working on recreating the site, it was a good lesson learned in regard to what can happen if not working correctly within the terminal. I am grateful that this happened in an earlier project in my coding career, than with a larger project where it could have been more damaging. 