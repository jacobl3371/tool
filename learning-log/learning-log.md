3/4/24

    - Used TailwindCSS to create a responsive navbar webpage
        - Collapses the displayed links on the navbar
        - Affected when the screen size is less than or equal to medium
        - Those links are hidden within the toggleable menu icon
        - When the menu icon is toggled the collapsed elements appear
        - The icon also turns into a close button
            - This requires some javascript
            - I used [this video](https://www.youtube.com/watch?v=X6CsbhSVUEc) for the setup
            - The Javascript which was provided did not work
            - The menu icon wasn't even toggleable
        - Since I couldn't find any documentation I had to use a code debugger similar to Replit
        - This did help me understand somewhat better how the tool works
        - Aswell as how to incorporate it into HTML, CSS and Javascript
            - In the future though, I must utilize the Slack channel for TailwindCSS
            - I will use it to ask any questions and debug my code
            - Which will help me understand it a lot better than an automated debugger
        - Available at: https://jacobl3371.github.io/tool/
        - Next Steps:
            - Try to setup a webpage/website components using TailwindCSS
            - Doing this by *only* watching or reading documentation
            - If I really can't figure it out, I will **ask the slack channel**


3/11/24

    - I learned on my own how to create a carousel in TailwindCSS
        - Following [this tutorial](https://www.youtube.com/watch?v=QXUM_AycJEc)
        - At [this point](https://youtu.be/QXUM_AycJEc?si=eUoUFKJAeCWoR2an&t=408) in the video I changed the img class
            - I only set the class to cover instead of h-full and w-full as well
            - The cover option worked better for my image
            - I couldn't get the image used in the video since it is not a link
            - The image was n the form of a file which existed locally
            - Either in their account-based IDE or on their hard drive (VS code desktop)
        - When adding the other two images for the carousel I had to add back the w-full and h-full classes
            - But I had to remove the object-cover class to keep the images from overlapping
            - This also made each image take up a proportionate height and width
        - At this point my h2 elements were all overlapping since they were in the center of the page
            - I ultimately got rid of the headings
            - The video explained everything else except for how to add the headings properly
        - [Result](carousel.html)


3/16/24

    - Used Tailwind and Javascript to create a multi-card slideshow carousel
        - Followed [this code](https://github.com/JAFSCodeSchool/multi-card-carousel-using-tailwind-and-javascript/tree/master)
            - I replaced all of the instances of image 1, 2, and 3 in the html with the links to the raw github image files
            - Swapped the words: next and prev in JS button functions
            - This makes the left and right buttons scroll in their specified direction
            - I noticed that as soon as you click to scroll, it brings you back. So you have to click twice just to even scroll once
            - Let alone the fact that there is a few second timeout in which the slide goes back to the previous one after clicking
            - The user can click very fast to get from Heading 1 to Heading 8
                - It is really annoying if they are clicking at a *constant* not-fast-enough-speed
                    - Especially after heading 4
                - If the user doesn't click fast enough they will be sent to the previous slide in an instant
                    - At least if they click very fast they don't get interrupted and pushed back mid-scroll
                - I was tinkering around with the code
                - The first line of Javascript

                ```
                let sliderContainer = document.getElementById('sliderContainer');
                ```

                - Can have the code within the parenthesis changed to only slider to reference only the ul element the elements forming the cards are inside and not the overlaying div
                    - Making no difference in the output


