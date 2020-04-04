# Today's Objective: Live CSS Editor

## Prize

$25 CAD Amazon gift card + bragging rights.

Tip: Read the [General Information Document](General%20Information.md) for more info on how to get started and submit.

## Objective

Today's objective is to create an in-site CSS editor of your own design.

Live CSS editors are handy tools that let you edit a website's styling in realtime. They are indispensible when building design-heavy websites, letting you iterate quickly through several different versions of a design before deciding what version you want to keep.

Quick flashback: In 2017, I built a CSS editor that could edit the look of a website on the fly. [You can still find it on the Chrome extension webstore](https://chrome.google.com/webstore/detail/navi-live-css-editor/cbiegoddgmmhbaompgcnkhjgonpkpogc). I named it after my wife, Navi (who is also involved with Mintbean, by the way). browniePoints++ :-)

## Requirements - NOT a Chrome Extension

So, this is your task:

Create a CSS Editor. When you type some CSS in the editor, it is immediately applied to the current website.

You do NOT need to build a Chrome Extension. You can build this right inside a web application.

Let's talk about the architecture.

### Architecture

There are 3 components you need here.

First, you need an input field where you'll write code. This is either a plain textbox, a `div` with the `contenteditable` attribute, or a full-fledged library-driven editor like Ace or CodeMirror. See below for suggestions.

Second, you need some kind of onChange listener that listens for changes to the input field.

Third, you need a `style` tag that contains and gets updated with CSS. All you should have to do is output your CSS into the `style` tag's innerHTML, and the browser should pick it up immediately. 

Tada! CSS Editor!

## Library suggestions

Let's talk about what you can use to build this.

You should definitely NOT build a backend component for this project. This project is very easy to implement, and can be done with a simple HTML page and some JS files.

Also, building a code editor from scratch is NOT recommended. Features like error-checking, linting, syntax highlighting, theming, and the like are very advanced and completely out of scope for this Hackathon. Instead, you might consider using a library.

I've used the following libraries to do stuff like this, and they work pretty well:
* Option 1: Ace Editor (easier and more polished. recommended for most people.)
* Option 2: CodeMirror (slightly harder but more customizable, and fully open source)

BUT! If using a library seems daunting, you can just use a plain textbox!
* Option 3, for newbies: Use a plain textbox to write CSS in. No need to implement any advanced features at all :-)

The design can be of your own choosing, and so this project is very open-ended.

### Bonus Points: Package it as a Chrome Extension and upload a video

Feeling gutsy? Want to do something out-of-the-ordinary?

Building a chrome extension will get you extra points in Aesthetics and Code Quality. But please, only attempt it if you are confident about it :-) It can be tricky the first time around.

You've already seen the extension I built: [Navi Live CSS Editor](https://chrome.google.com/webstore/detail/navi-live-css-editor/cbiegoddgmmhbaompgcnkhjgonpkpogc). Here are some other examples of CSS editors that are chrome extensions.

* [Amino](https://chrome.google.com/webstore/detail/amino-live-css-editor/pbcpfbcibpcbfbmddogfhcijfpboeaaf?hl=en-GB)
* [Live CSS Editor](http://www.livecsseditor.com/)
* [Visual CSS Editor](https://chrome.google.com/webstore/detail/visual-css-editor/mibmnbcmaafgepannenjiemibkojedam) (this one is more GUI-driven)

## Restrictions

* Your project must use JavaScript.
* Your project must NOT have a backend component. (It really isn't needed)
* FOR WEBSITE-ONLY PROJECTS: You must deploy your project online.
* FOR CHROME EXTENSIONS: `IMPORTANT` For security purposes, I will NOT be installing anyone's extensions on my local machine. To get aesthetic points for your extension, please upload a 1 to 2 minute video of you using the extension to edit a 3rd party website.

There are no other restrictions.

## Tips for success:

1. The project is intentionally simple so you can focus on code quality.
1. The requirements are intentionally minimalistic so you can get as creative as you'd like.
1. You get a LOT of time for code review comments. So you can win even if you feel your project isn't great, simply on the strength of your code review comments!
1. Keep in mind, 33% of your score is based on aesthetic appeal! So try to make it look nice.
