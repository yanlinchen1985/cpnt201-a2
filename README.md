# Cpnt201-a2 -Blog home page

by  Lynn Chen     Oct,16,2020



This project is about the website of a Chinese Restaurant named "Panda's kitchen", which specializes in traditional Chinese food. In this Blog home page, there are 5 different Chinses food from its menu with photos and Introductions, which can help viewers know more about this restaurant's dishes.



## Comments

There are some issues when I optimized the images. These photos come from my family meals these days. I took them with the SLR, so source photos' width and height are 6240px and 4160px. When I optimized them, it was difficult to compress them under 100Kb with 2000px width high quality images.

The other problem when I wanted to display them at their respective viewport widths. I used the srcset to do it, but I did it by using small image in our class blog task. However, this time I need to use the medium image set as the src attribute fallback.  

I set it like : 

> ​     srcset="
>
> ​     images/sm/dumpling.jpg 500w,
>
> ​     images/md/dumpling.jpg 1000w,
>
> ​     images/lrg/dumpling.jpg 2000w,"

Because I thought that the number before w seems like the width of the photos, even though one use w and another use px as units. However it could not work well, and it only has the large and meddle sizes to display.

Therefore, I compared the numbers in your demo webpage ( [monkey changes color](https://sait-wbdv.github.io/sample-code/frontend/image-performance/srcset/)) created in our class that you also used 750,1500 and 2000w in srcset. The width of the monkey's images are 500px,1000px and 2000px. 

Then I tried like :

> ​     srcset="
>
> ​     images/sm/dumpling.jpg 750w,
>
> ​     images/md/dumpling.jpg 1250w,
>
> ​     images/lrg/dumpling.jpg 2000w,"

Boom! It works well this time! 

So I double checked and reviewed this point on CSS-TRICKS  [#133: Figuring Out Responsive Images](https://css-tricks.com/video-screencasts/133-figuring-responsive-images/)  and MDN [Responsive images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)

> ...Note that this uses the `w` unit, not `px` as you might expect. This is the image's real size, which can be found by inspecting the image file on your computer .

I did not spend too much time in the articles and their layout. I think how to ensure all the images in different screen sizes to work well is the point of this assessment,so What I did more was trying again and again to adjust. I realize there are still many things I need to fix in this assessment,especially in **responsive optimization**.



## Attributions

Some Code in this project come from MDN and Tony Grimes's  sample code in class  [SAIT WBDV](https://sait-wbdv.github.io/) 

like: https://sait-wbdv.github.io/sample-code/frontend/image-performance/srcset/,



## Webpage 

GH repo: 

GH Pages website: 



Thank you.