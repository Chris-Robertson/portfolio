# Chris Robertson - Developer Portfolio Website

https://chris-robertson.github.io/portfolio/

## Brief
This portfolio website was made as our first major project when I was studying at CoderFactory Academy coding bootcamp. The brief was to simply create a responsive website that could be shown to prospective employers in the future. It should showcase any projects that I have created, as well as contain an about bio and ways to contact me.

## Restrictions
I restricted myself to only using plain HTML and CSS. While I am aware that there are many, many frameworks, boilerplates and languages that can be used to make website development easier and more powerfull, I wanted to restrict myself to only the basics. My reasoning was that I would better understand the use of these framworks if I had a fuller idea of the underlaying technology that they are augmenting.

## Inspiration
At the time I was listening to a lot of 80s-style retro synthwave music and was heavily inspired by the neon-infused gaudy style of the era. I felt that creating a bold design from these influences would inject some of my personality into the site and help it stand out from the ususal minimalist software developer fare.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=MV_3Dpw-BRY
" target="_blank"><img src="http://img.youtube.com/vi/MV_3Dpw-BRY/0.jpg" 
alt="Kavinsky - Nightcall" width="400" height="270" border="10" /></a>

I collected inspirational images into a board on [niice.co](https://niice.co/m/4dbeb203f69cb87f0b3b8c04d6e8d6d7)
From these images I created an idea for the colour palette I would aim for.

<img src="https://github.com/Chris-Robertson/portfolio/blob/master/images/readme/niice_inspiration_board.png" alt="niice.co inspiration board" width="400" />

<img src="https://github.com/Chris-Robertson/portfolio/blob/master/images/readme/colour_gradient.png" alt="Colour Palette" width="400" />

I found an [80s text generator](https://m.photofunia.com/effects/retro-wave) online that I used to create a placeholder theme reference.

<img src="https://github.com/Chris-Robertson/portfolio/blob/master/images/readme/theme.png" alt="Theme Guide" width="400" />

## Planning
From here I started the wireframing and blocking out of the content using the online service [Figma](https://www.figma.com).

I had never used a tool like this. In the past I would just knuckle in an start coding without much consideration or planning. This, of course, is a less than efficient way of doing things. I found that using Figma I was able to quickly and easily produce something that I was happy with that could be turned into HTML.

I found particular value in being able to iterate through designs. After producing a very basic wireframe of the site layout, I duplicated it and added further details.

<img src="https://github.com/Chris-Robertson/portfolio/blob/master/images/readme/figma_project.png" alt="Figma Mockups" width="400" />

## Construction
Once the site mockup was complete it was time to start building it. To help keep me organised I used a [Trello](https://trello.com/) board. Here I created a lost of things that needed to be completed . I would add to the list over time as I thought of new ideas or was given new inspiration. The board continues to serve as a TODO for the site, keeping track of features and changes I would like to make in the future.

<img src="https://github.com/Chris-Robertson/portfolio/blob/master/images/readme/portfolio_trello.png" alt="Trello TODO List" width="400" />

### Responsiveness
One of the requirements for the site was for it to be responsive over multiple devices. To aid in this I adopted a "mobile first" design approach, planning out the site for the smaller screen sizes first, before scaling everything up to larger sizes. The aim of this approach is to both ensure that the site is properly displayed on the most popular screen sizes (mobile) as well as to keep to code iteself simpler and more concise.

Here is one of the first iterations of my respnsive design. Can you tell I was still a novice with Chrome Developer Tools?

<img src="https://github.com/Chris-Robertson/portfolio/blob/master/images/readme/responsive_design_01.gif" alt="Responsive design" width="400" />

### Parallax
I had decided early in the process that I wanted parallax elements in my site. I felt implementing this in pure CSS with no Javascript tricks would be a good test of my skills and a great learning experience. Inspired by various images in my Niice board, I also decided not just on rectangular parallax elements, but on hand-made, transparent graphics of different shapes and sizes. This required me to dust of my Adobe suite skills and start drawing.

Here is an initial test of my parallax CSS code and some of my custom images. It was around here that the difficulties I had set myself up for started to appear. 

<img src="https://github.com/Chris-Robertson/portfolio/blob/master/images/readme/parallax_testing_01.gif" alt="Parallax Testing" width="400" />

My technique for creating the parallax effect was to transform elements along the z-axis. This creates the perspective difference for objects to move at different speeds relative to each other. The problem with this is that as you move elements around the z-axis they become larger or smaller. As I had moved the text elements back, they had become smaller, so I scaled them up to retain their initial size, but to still move slower compared to the closer elements. This technique worked fine untill I tried to implement some internal links.

My initial plan was to have link buttons at the top of the site that would fst-scroll to the various sections. However, as I was linking to elements whose scale and position had been altered, the anchors turned out to be in unreliable locations.

<img src="https://github.com/Chris-Robertson/portfolio/blob/master/images/readme/jump_links_broken_01.gif" alt="Broken internal page links" width="400" />

A possible solution to this problem would be to fix some anchor divs at the various locations around the site and link to them. I decided in the end that the jump buttons were really unneccessary and I removed them. This site is short enough that scrolling through wasn't taking too long, and I would prefer to implement a slicker navigation system in the future.

The major problem with my implementation of parallax was the positioning of objects. Because I wanted the timing of when a parallax object came onto the screen and when it left to be exact, the object had to be positioned exactly. This completely broke when adjusting to larger screen sizes, requiring me to use many media queries for various resolutions, a less than ideal approach.

## Learnings
Over the course of building this site I have exponetially increased my knowledge of CSS and have realised that there is so much more to this 'language' that I need to learn.

The way I approached implementing parallax in CSS was ultimately flawed. As the site sits now, it is responsive over the most popular screen sizes, but is not 100% dynamically responsive. Towards the end of the project, as the deadline loomed, I understood ways that I could remedy these faults. This would, however, require an almost complete re-write of the CSS. As time was running out, I decided to keep the site as it was, partially-responsive. Done is better than perfect, as they say. In the future this is something I will definitely revisit and implement, as well as a slew of ideas accumulating on my Trello board.

Throughout the project I often found myself unhappy and dissatisfied with the general design of my site. I didn't like the colours, or the graphics I had made. I wasn't happy with the font, or the text, or how the entire site flowed. I couldn't seem to rectify these ideas I had in my head with what I was actually able to create.

We were shown a quote earlier in the course from Ira Glass, and I reminded myself of it often. This was one of my first serious web design projects. It's unrealistic to expect myself to knock it out of the park and compete with the professionals who have been doing this for years. Instead I have made my self acknowledge to progress I have made and the things I have learned, and I have resolved to keep updating this portfolio as my skills increase until it is something that I can be proud of.

<img src="https://github.com/Chris-Robertson/portfolio/blob/master/images/readme/ira_glass_quote_02.gif" alt="Ira Glass Quote" width="400" />

