---
layout: default
title: Maintaining this Website
---

# Maintaining this Website

A guide for myself on how to maintain and update this website.

## Adding a New Entry

1. Add the entry to main page
    - Open the catagory markdown page (either projects, trip reports, or evergreen) that corrosponds to the new entry
    - Copy and paste existing entry, edit title and dates
    - Edit hyperlink to ``` page_title/page_title.html ``` (make sure the name the file type is ```.html```, not ```.md```)
2. Create the entry
    - Under the folder titled corrosponding to the catagory (either projects, trip reports, or evergreen), create a new folder with the name of the entry
    - Within the new folder, create a markdown page with the same name.
    - For example, BLiMS has ```projects/blims/blims.md```
3. Set up the page
    1. Add the following header:  

        ```markdown
        ---  
            layout: default  
            title: page_title  
        ---  
    
        # page_title  
        ```
4. Edit the page
    - Generate live preview
        - ```jekyll serve```
        - Note this must be run from the ```thomas-rimer.github.io``` directory
        - Navigate to ```localhost:4000``` to view the live preview
    - All resources related to that page (photos, videos, PDFs, etc...) go within the folder with the related name
    - Hyperlinks relative to the page (to files outside the page's own direcotry) must be prefixed with ../../ to reach what you see as the base directory. For an example, see the code for the example video on this page.
5. Push to GitHub. Type the following into the commandline
    1. ```git add .```
    2. ```git commit -m "added XXX project page"```
    3. ```git push```
    4. Enter password and hit enter
    5. It will upload to GitHub, and should be viewable within a few minutes

## Markdown Syntax

### Inserting Special Objects
Drag the file into the folder corrosponding to the page (i.e. ```projects/blims```). Then rename it to something friendly. Because .md pages are saved in the folder, you can access them simply by their name (i.e. the path to ```blim_3.2.png``` would just be ```blims_3.2.png```).

#### Images
```alt``` is for text that shows up if the image can't load. See the section below on creating new classes for image customization. Figcaption can be left blank for no caption.

```html
<figure class="center-figure">
    <img src="blims_2.png" alt="">
    <figcaption>Photo of the assembled BLiMS</figcaption>
</figure>
```

<figure class="center-figure">
    <img src="../../projects/blims/blims_3.2.png" alt="">
    <figcaption>Example image</figcaption>
</figure>

#### Videos
Process is pretty much identical to photos. Make sure the video is mp4 format (you can simply rename ```.mov``` to ```.mp4```). Note ```jekyll serve``` often has issues with videos, but they resolve themselves when pushed to GitHub (or when viewed on Safari). GitHub does not allow large videos, to be safe ensure the video is under 25 MB.

```html
<figure class="center-video">
    <video controls autoplay loop muted>
    <source src="../../projects/blims/blims_launch.mp4" type="video/mp4">
    Your browser does not support the HTML5 Video element.
    </video>
    <figcaption>Rocket launch</figcaption>
</figure>
```

<figure class="center-video">
    <video controls autoplay loop muted>
    <source src="../../projects/blims/blims_launch.mp4" type="video/mp4">
    Your browser does not support the HTML5 Video element.
    </video>
    <figcaption>Example Video</figcaption>
</figure>

#### PDFs
I found 500x700 fits google doc exports well.

<object data="../../projects/blims/blims_tech_report.pdf" type="application/pdf" width="500px" height="700px">
    <embed src="../../projects/blims/blims_tech_report.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="../../projects/blims/blims_tech_report.pdf">Download PDF</a>.</p>
    </embed>
</object>

### Basic Syntax

| Name    | Example | Code |
| -------- | ------- | ------- | 
| Bold text | **bold text** | ```**bold text**``` |
| Italic text | *italic text* | ```*italic text*``` |
| Underline text | <u>underline text</u> | ```<u>underline text</u>``` |
| Code block | ```code = block()``` | ```` ```code = block()``` ```` |
| Largest Title | - | ```#Largest Title``` |
| Medium Title | - | ```##Medium Title``` |
| Small Title | - | ```###Small Title``` |