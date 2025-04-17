# Band Documentation 
[Our Band Site](https://nickreinert.github.io/)

We started by using the sample website as a [template](https://kariestes.github.io/) to use for our band site. We viewed the source code which looked like this...

`<html>
<head>
  <title>Band Website</title>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
  <header>
      <h1>Three Monks of "<i>Mass.</i>"</h1>
  </header>
<meta charset="utf-8">
<body>
  <h1>About Us</h1>
  <p>We are the Three Monks of Mass. With a passion for Gregorian Chant music,
  we are in production for our 29th album, "One Hot Mass". Consisting of three soprano
  monks, this band is working to change the face of Gregorian Music in monestaries around the world.
  <b>Check out our hit single "Wonder Chant"</b>
  </p>
  <p>
  <audio src="Wonderwall.mp3" controls>
  </p>
<h1>The Band</h1>
<img src="Monks.png" alt="The Band">
<h3>Meet Father Kari</h3>
<p>Father Kari resides from deep in the forests of rural Illinois. Growing up in
a hut, she found her passion for singing when she was asked to call her many dogs
back to the house for supper. She joined the monks after her family left her
at the gas station at the age of 3. Since then, she has taken the role as back-up
to the back-up lead soprano singer, and plans on staying in that position until she dies.
</p>
    <h3>Meet Father Thomas</h3>
    <p>Father Thomas, a Malibu native, is well-renowned for his soaring soprano range and facility. He joined the group in 2017 for their Chant-pionship win at the 1252th annual Chant-off where the group chanted for record 30 hours straight. In addition to chanting, Father Thomas also enjoys a good yodel, and got his undergraduate degree in polyphonic yodeling from NYU in 2016.</p>

    <h3>Meet Father Noah</h3>
      <p>Father Noah is a native to Finland, currently residing in Rome.
      Father Noah found his calling during the 10th century
      when the pope gave a decree that gregorian chanters
      would be paid a fair living wage and given respectable royalties on all chants!
      Despite the advent of the influential politician spotifius maximus, Father Noah
      has been a strong leader at the center of equal opportunity for gregorian chanters.
      Some of father Noah's favorite hobbies are taking care of the garden at the local
      monastery, going for long walks on the tiber river, and painting natural landscapes.
    </p>

      <h3>Reviews</h3>
      <p>"the hottest monastery of the 12th century"</p>
      <p>"a group that will make you go, 'oooh!'"</p>
      <p>"I took my kids to see <i>One Hot Mass.</i>, the chants are kid friendly and easy to sing
          , fun for the whole family!"</p>
      <p>"the performance was enchanting, divine, and spiritually captivating"</p>

</body>
</html>
`
## Problem
We made sure to make our own styles.css file and we wanted to make an image a background for our website instead of just a basic color. We had some issues with getting our image to show as the background because we tried using a url of the image from the internet. Even though we had put the image in the same folder as our index.html file it wasnt working. So then we checked a [source online](https://www.w3schools.com/css/css_background_image.asp) for help and realized we should just use the name of the image file exactly as it was in the folder on our computer. The the image worked for our background. 

##Changes We Made
After we figured out the background image everything went smoothly. We just replaced the text with our band information. We also used our own mp3 that we found from [Splice](https://sounds.splice.com/plans?utm_source=google&utm_medium=cpc&utm_campaign=namer-en_multi_gs_ua_sounds_20220602_brand_trials&utm_content=namer-en_multi_gs_kw_brand-splice_x_x_x_exact&utm_term=splice&campaignid=404596759&adgroupid=26303056279&adid=696954328285&gad_source=1&gclid=Cj0KCQjwzYLABhD4ARIsALySuCQF83bKd3ZHrB2KJzsJqOcp2g3Fm9RzDCA9NVlzMO6UMNJZFlYjqqUaAndcEALw_wcB). Similarly, to input the image as the background in the css file, to do the audio file, we just used the same name as the audio file in the folder with the index.html file. We also added a band image that Annie had Photoshopped and kept its large size to push down our text into the lighter part of the image so our band bios were readable. We called the audio file and band image in the html file but then we went back into the .css file to change the font to Papyrus. We also then deleted the Reviews from the original in the html file since we didn't want reviews on our own site. Here is the code for our html file...

`
<html>
<head>
  <title>Band Website</title>
  <link rel="stylesheet" type="text/css" href="styles.css">
</head>
  <header>
      <h1>Reject Society; Return <b>2</b> Nature</h1>
  </header>
<meta charset="utf-8">
<body>
  <h1>What We Stand For</h1>
  <p> We are a band <i>and</i> philisophical group. We value all carbon based matter, algea, snail, mushroom, cucumber (sea), cucumber (land), pickle, chicken, luke skywalker, vulture, grass, black mold, sea urchin, mosquito eater, wasp larvae, and maggot.
  <b>This is a special piece, dedicated to trees. Take a breath, and take a listen.</b>
  </p>
  <p>
  <audio src="ForestMorningBirds_SFXB.75.wav" controls>
  </p>
<h1>The Group</h1>
<img src="Programming Band.JPEG" alt="The Group">
<h3>Sarah</h3>
<p>Sarah, a native of the ocean, is well renowned for crafting mystical melodies from the high winds above the Pacfic. She holds a master's degree from Stanford University in aquatics and improvisational performance. Sarah has been in the band since 1857. 
</p>
    <h3>Nick</h3>
    <p>Nick is a squirell known for his profound ability to make music with nuts of all kinds. Coming from Tanzania, he learned to play the walnut at a young age, and later picked up the almond. He was awarded a Grammy for his performance on "Nuts from around the Globe."</p>

    <h3>Father Malcolm</h3>
      <p>Malcolm is a human from the forest. He was born and raised in the forest. He got his undergraduate degree in eating food, with a minor in advanced neurochemistry. He currently resides in a forest.
    </p>
	
    <h3>Annie Spade</h3>
      <p>Annie, a land dweller who is a fan of the Pacific ocean. She studies aquatics and fish of the local land. Residing in the sunny beaches in the south of California, she can be found studying the mythics of the Sea.
    </p>

      <h3>Reviews</h3>
      <p>""</p>
      <p>"a group that will make you go, 'oooh!'"</p>
      <p>"I took my kids to see <i>One Hot Mass.</i>, the chants are kid friendly and easy to sing
          , fun for the whole family!"</p>
      <p>"the performance was enchanting, divine, and spiritually captivating"</p>

</body>
</html>
`
And here is the code for our styles.css file...
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
## Self-Assesment
I to contributed the group by finding the [resource online](https://www.w3schools.com/css/css_background_image.asp) that showed how to call on the image in the styles.css file. I also contributed to my own band member bio and helped brainstorm ideas for the audio file and general band bio. 

##Group Assesment
Annie: Annie photoshopped our group photo and inspired us to make an image for the background of our website. She also contributed to her individual bio and helped brainstorm ideas for the band's theme. 

Nick: Nick hosted the site, chose the photo for the background, and changed the font in the styles.css file He also contributed to the individual bio and equally helped brainstorm our band's brand. 

Malcolm: Malcolm contributed to his individual bio and also was instrumental in coming up with our band's nature concept and suggested to use a nature related audio file.

I feel like we all equally contributed to coming up with the creative aspects of our website as well as the technical coding side of the assignment. We all tried to troubleshoot and figure out why the image wasn't working as the background before reffering to the outside resource. 