live URL - 

# Resources:
https://www.youtube.com/watch?v=exb2ab72Xhs
https://www.youtube.com/watch?v=l6sxh57ifSQ&t=789s
https://i.ytimg.com/an_webp/OtBpgtqrjyo/mqdefault_6s.webp?du=3000&sqp=CMzg2JcG&rs=AOn4CLA9yJe7ry4iW7Tr1POFbMg1A6z49w
https://www.youtube.com/watch?v=e1KpKBHJOrA


# learnings
CSS image overlay
box shadow
inset

# TO_DO
CSS image overlay
box shadow

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
