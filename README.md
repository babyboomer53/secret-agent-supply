# secret-agent-supply
Codecademy's Build Websites from Scratch – Unit 5

Wow! A word to the wise.

I've been working on one of the BWS projects for longer than I care to admit. For a particularly troublesome section, I decided I take advantage of the tools offered by CodePen, so I finished the development there. The next step was to stitch the code I developed outside of CodePen to the code I had developed in CodePen. Before commencing the stitching process, I created a new Git branch so that I could easily revert to a point where both halves of the code were known to be working. I wasn't expecting it to be easy; merging HTML and CSS files can be tricky.

I worked my way through the code, tackling each bug as I encountered it. The HTML was pretty solid, so most fixes involved tweaking the CSS file. Eventually I encountered one particularly vexing problem. I had an element that had collapsed, so I knew that it needed a height property. I found the place in the code where I had addressed the problem before, and couldn't figure out why it had suddenly stopped working. I asked myself, "What role takes precedence over an in-line style rule?" That's when it occurred to me. It had to be the reset file! So, I disabled the reset file. Voilà!

The reason the code worked in CodePen is because in that environment I hadn't had to contend with the reset file. I wondered whether it would be worthwhile trying to refine my rules to override the reset file. While that might be a worthwhile exercise for a future project, I had already spent a couple of hours fighting a losing battle. The reset file had to go!

I started the project using the Brackets code editor. Since beginning this journey less than two months ago, I've already tried about four editors. I have yet to find one that has everything, but like CodePen, Brackets also has a live preview. It also includes a feature which allows me to edit an element's corresponding CSS rules without switching files. Additionally, there are a number of open source extensions that can be installed to provide Git and GitHub integration.

It's too early for me to know which editor I prefer. Currently, I bounce back and forth between a number of them. All of them have features in common. I usually pick the one that serves my purposes at that time. But I digress…

This is the second time I've gotten into conflict with the reset file. I'm hoping it will be the last.

Yesterday, the Brackets "Live Preview" feature developed a glitch. The symptom is that several seconds after opening the document in my default browser, the live preview closes with the following message: "(Brackets Live Preview: closed)."

I reinstalled Brackets, but the symptoms persisted.

During the last few days, Brackets behavior has become more erratic. During that period I had installed a couple of extensions. Those extensions were Beautify 2.5.2, Brackets unGit 1.4.22, HTML Skeleton 1.4.3 and W3C Validation (by Umoxfo) 1.1.0. I disabled all of them, and the Live Preview function was restored! To identify the culprit, I decided to disable the extensions, one at a time. I started with the W3C validation extension. Once again, normal functionality of the Live Preview feature was restored! It appeared as though I had identified the culprit on the first attempt.

I'd been using the W3C validator for several days without issue. I'm not sure why it would suddenly start giving me problems. A few days ago I moved my project from my local system to CodePen. Perhaps the problem with Brackets hadn't had an opportunity to reveal itself.

All is well that ends well, but I've lost the built-in validator in the process. I guess one option I have is to enable the validator when I don't need Live Preview.

I spent all morning and half of the afternoon trying to impllement a "sticky" navigation bar in the browser. I found a couple of examples on the Internet, of which I tried two. The one I ended up using had the fewest lines of code (not necessarily a selection criterion), and was found at https://www.w3schools.com/howto/howto_js_navbar_sticky.asp. In the end, it was the Z-index property that came to the rescue! Until I applied that property to the element I wanted sticking to the top of the page, it kept scrolling out of sight.
