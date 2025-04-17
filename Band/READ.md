# Band Documentation 
[Our Band Site](https://nickreinert.github.io/)

We started by using the sample website as a [template](https://kariestes.github.io/) to use for our band site. We viewed the source code and filled in our own information about our band and our own files.


## Problem
We made sure to make our own styles.css file and we wanted to make an image a background for our website instead of just a basic color. We had some issues with getting our image to show as the background because we tried using a url of the image from the internet. Even though we had put the image in the same folder as our index.html file it wasnt working. So then we checked a [source online](https://www.w3schools.com/css/css_background_image.asp) for help and realized we should just use the name of the image file exactly as it was in the folder on our computer. The the image worked for our background. This is what it looked like in our css file...
`
body {
  background-image: url("free-nature-images.jpg");
background-size: cover;
background-repeat: no-repeat;
}

h1 {
  color: black;
  text-align: center;
  font-family: "Papyrus";
}

h3 {
  color: black;
  text-align: center;
  font-family: "Papyrus";
}

p {
  font-family: "Papyrus";
  font-size: 20px;
  width: 800px;
  margin: 0 auto;
  text-align: center;
}
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
header
h1 {
  font-family: "Papyrus";
}
`

## Changes We Made
After we figured out the background image everything went smoothly. We just replaced the text with our band information. We also used our own mp3 that we found from [Splice](https://sounds.splice.com/plans?utm_source=google&utm_medium=cpc&utm_campaign=namer-en_multi_gs_ua_sounds_20220602_brand_trials&utm_content=namer-en_multi_gs_kw_brand-splice_x_x_x_exact&utm_term=splice&campaignid=404596759&adgroupid=26303056279&adid=696954328285&gad_source=1&gclid=Cj0KCQjwzYLABhD4ARIsALySuCQF83bKd3ZHrB2KJzsJqOcp2g3Fm9RzDCA9NVlzMO6UMNJZFlYjqqUaAndcEALw_wcB). Similarly, to input the image as the background in the css file, to do the audio file, we just used the same name as the audio file in the folder with the index.html file. We also added a band image that Annie had Photoshopped and kept its large size to push down our text into the lighter part of the image so our band bios were readable. We called the audio file and band image in the html file but then we went back into the .css file to change the font to Papyrus. We also then deleted the Reviews from the original in the html file since we didn't want reviews on our own site. 

## Self-Assesment
I contributed to the group by finding the [resource online](https://www.w3schools.com/css/css_background_image.asp) that showed how to call on the image in the styles.css file. I also contributed to my own band member bio and helped brainstorm ideas for the audio file and general band bio. 

## Group Assesment
Annie: Annie photoshopped our group photo and inspired us to make an image for the background of our website. She also contributed to her individual bio and helped brainstorm ideas for the band's theme. 

Nick: Nick hosted the site, chose the photo for the background, and changed the font in the styles.css file He also contributed to the individual bio and equally helped brainstorm our band's brand. 

Malcolm: Malcolm contributed to his individual bio and also was instrumental in coming up with our band's nature concept and suggested to use a nature related audio file.

I feel like we all equally contributed to coming up with the creative aspects of our website as well as the technical coding side of the assignment. We all tried to troubleshoot and figure out why the image wasn't working as the background before reffering to the outside resource. 