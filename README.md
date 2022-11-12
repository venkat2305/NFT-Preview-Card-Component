live URL - 

# Resources:
https://www.youtube.com/watch?v=exb2ab72Xhs
https://www.youtube.com/watch?v=l6sxh57ifSQ&t=789s
https://i.ytimg.com/an_webp/OtBpgtqrjyo/mqdefault_6s.webp?du=3000&sqp=CMzg2JcG&rs=AOn4CLA9yJe7ry4iW7Tr1POFbMg1A6z49w
https://www.youtube.com/watch?v=e1KpKBHJOrA


# learnings
1. CSS image overlay
2. box shadow
3. inset
1. Most important on this is actually getting the html right. There are some essential steps that have to be taken for this to work for all users (eg mouse, keyboard, screenreader)
2. Wrap in an anchor tag (or button depending on what you would expect clicking on it to do) that’s display block and position relative. Give it an aria label
3. Have your image inside that also set to display block max width 100%. Make it have an empty alt
4. Add a before and after pseudo element to the anchor tag, absolutely positioned and 100% width and height and keep their content in css as an empty string
5. Make one pseudo background color teal
6. Make the other background image with the eye image. Use background properties to size and position itcentrally
7. Set both to have opacity 0 by default
8. On hover of the anchor (link) make the pseudo with teal color opacity 0.7ish, make the pseudo with the eye opacity 0.
9. You may need to use zindex on the pseudos to make them.stack correctly
10. You may want to add in transition properties to make the change smooth (edited) 

# TO_DO
CSS image overlay
box shadow

fix hover with psuedo elements 

reference code - https://github.com/A-C-Sai/nft-preview-card-component/blob/main/styles.css


https://frontendmentor.slack.com/archives/CCYHFT85B/p1641799633029300?thread_ts=1641799037.017200&cid=CCYHFT85B

I would use pseudo elements for this
wrap img in an anchor tag set to display block and position absolute
Set img to display block too
Pseudo on the anchor tag (:before or :after or both)
Have the pseudo be 100% width and height and teal background color, opacity 0
The eye icon can be a background img on the same pseudo but means you have to change the hsl teal color to hsla so it's opaque. If you don't want to change the hsl color place the eye icon on a different pseudo
On hover of the anchor tag, set opacity on pseudo to 1 (or 0.7ish if teal color is in its own pseudo and hsl)
You may want to add a transition opacity to them
You may need to use z-index to later the pseudos on top of each other (one with eye icon in would need to sit on top)
Make sure the anchor tag has a label either by including Sr-only text or aria label or alt text on the image
