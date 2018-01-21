# Week1&2 Checkpoint

DGM6410 Game Design Tech Lab

This repository contains:

<ul>
  <li>Updated Game file(.html page)</li>
  <li>Media files(sound, img)</li>
 
<li>Supplementary docmentations:<ol>
<li>Inquiry</li>
<li>ResearchPlan</li>
<li>Solution</li>
<li>Expectation</li>
</ol></li>

</ul>

Based on previous project <a href="https://github.com/appleseed0910/Hello-There">"HelloThere"</a> (an interactive fiction made by Twine2.0)


<br>
<h2>Supplementary Documents</h2>
<br>
<h3>Inquiry</h3>
Customize my Twine story in different aspects. It contains:
<ul>
  <li>Remove the "Back" button</li>
  <li>Add a "Start" Page</li>
  <li>Add "Save" and "Continue" functions</li>
  <li>Add background sound effect</li>
  <li>Adjust the entire layout</li>
  <li>Give 'Bookmark' a specific style</li>
  <li>Add title imgae on the Start Page</li>
  </ul>
  
<h3>ResearchPlan</h3>
Search online tutorials, and embed the revision into the project, test.

<h3>Solution</h3>
Here are some tutorials and solutions I found for each inquiry.
<br><br>
<ol>
  <li><b>Remove the "Back" button</b>
<br>https://twinery.org/forum/discussion/2931/remove-back-option-in-2-0
<br>Since Twine uses CSS style sheet, for default story mode, we could set up the 'display' property of tw-sidebar as 'none'.
However, I think this would disturb if I put any elements inside tw-sidebar. I may need to figure out other solutions if needed.</li>

<br><li><b>Add a Start page</b>
<br>This one is comparatively easy, I added a new passage and set it as the Start Passage.</li>

<br><li><b>Add "Save" and "Continue"</b>
<br>I think it's important to have a "Continue" button on the start page to make the whole story is more like a game/friendly, since the story would be very long.
<br>(Although I think if there would be some "pop up" menu or floating menu, it would be better. My knowledge needs to be enhenced for reaching that level.)
<br>Right now, since the story hasn't been extended so long, I think single saving slot is enough. I deceided to use "Bookmark" as the saving link text. I haven't found a reliable way to add a saving code block to every passage, so instead, I might manually add them every 5 passages.
<br>https://twinery.org/wiki/harlowe:save-game
<br>https://www.youtube.com/watch?v=4YDeJ36diwc
<br>https://twinery.org/forum/discussion/4898/save-load-game-in-2-0-and-harlowe
  </li>
<br><li><b>Add Background Music</b>
<br>Since the story happens in a rainy night. I tried to add background music effect. But it terms out it's very handful to embed multi media in Twine(because we cannot write other type of file into a single html page! fair..)(I miss inkdML)
<br>https://twinery.org/wiki/twine2:add_an_image_movie_sound_effect_or_music
<br>https://www.youtube.com/watch?v=rkWkTJtK2dI&t=36s
<br>https://www.youtube.com/watch?v=aBG8Z-Lvfd4
<br>https://www.reddit.com/r/twinegames/comments/3lhh5a/background_music_in_harlowe/
<br>Here are some links that I've read for optional solutions. Technically, due to the limitations of Twine itself, it's hard to insert images or sound directly. We could use external link point to these files, but it's rare and sometimes illegal. I don't think this is a good choice?
<br>So,I tried optionB, stored the music file in the root directory with the story html file aside. Then inserted audio through simple html tag "&lang;audio src="light-rian.mp3" autopaly>&lang;/audio>".
<br>It works. However, as the Twine wiki said, relative links don't work inside Twine. So, for this way, it's necessary to revise the original code before we package the story.
<br>https://freesound.org/people/babusrelaxtv/sounds/344430/
<br>Here is the source of the rainy sound, it's in CC field.
  
  <br><li><b>Adjust the entire layout</b>
  <br>Through editing the internal CSS sheet, I adjusted the layout of the main text block on each passage. (It's easy once figured out that they are controlled by the same selectors 'tw-passage'. I also recovered the tw-sidebar elment. I think the default property of sidebar is significant if I want to put anything such as menu on all the pages. 
  <br>Instead, I set the display property of tw-icon as none which could stop the default arrow icons appearing. I've considered that if I want to create some icons, I guess I may try to write a new elment to arrange them.
  <br>https://furkleindustries.com/fictions/twine/twine2_resources/twine2_CSS_tutorial/
  <br>The way I use for layout gives enough margin visually, but it also takes space that I want to use for pictures. I may need return back once I done the preparation of pictures.
  
  
   <br><li><b>Give 'Bookmark' a specific style</b>
  Firstly, I created new Bookmark saving slots on

  
  
  </ol>

<h3>Expectation</h3>
Here are some potential inquiries for the next week.

