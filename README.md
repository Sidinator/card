# Card
HLS= Hue, Saturation, and Lightness <br>
1rem= most browsers sets default font size to 16px

# Challange:
https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ
# Link used:
### https://codepen.io/iamsofiullah/pen/wvdLJYN
Used this link to learn and understand how set the position of the SVG's in this project.

# CSS
    
#### Imports font family from googleapis
    @import url('https://fonts.googleapis.com/css2?family=Kumbh+Sans:wght@400;700&display=swap');
### Sets margin and padding to 0
    * {
    margin: 0;
    padding: 0;
    /* box-sizing: border-box; */
    }
### Sets fontfamily, background color and sets the body to flex
    body {
        font-family: 'Kumbh Sans', sans-serif;
        background-color: hsl(185, 75%, 39%);
        display: flex;
### Centers the card and sets the minimum height of the page to 100 viewe hight
        align-items: center; 
        min-height: 100vh;
### Adds background circles
        background-image: url('./img/bg-pattern-top.svg'), url('./img/bg-pattern-bottom.svg'); 
### Sets no repeat background and sets positioning of the circles (svg's)
        background-repeat: no-repeat, no-repeat;
        background-position: right 48vw bottom 40vh, left 45vw top 44vh;
    }
### Align all the text to the center within the container class
    .container {
        margin: 0 auto;
        text-align: center;
    }
### Sets the max width of the wrapper class, with a background color of white and adds a 15px border radius. Hides overflow and sets margin to 1 rem
    .wrapper {
        max-width: 420px;
        background-color: #fff;
        border-radius: 15px;
        overflow: hidden;
        margin: 1rem;
    }
### sets the width and height of the picture, aswell as sets a border radius as 50% (makes the picture round) aswell as adds a white solid border thats 4px wide
    .content img {
        width: 100px;
        height: 100px;
        border-radius: 50%;
        border: 4px solid #fff;

### sets the img up over the top background in the card
        margin-top: -52px;
        margin-bottom: 20px;
    }
### Sets the font color, font size, font to "bold" and margin for bottom for the h2 tag within the content class
    .content h2 {
        color: hsl(229, 23%, 23%);
        font-size: 18px;
        font-weight: 700;
        margin-bottom: 10px;
    }
### Sets the font color of the span tag within the content class h2 tag
    .content h2 span {
        color: hsl(227, 10%, 46%);
        font-weight: 400;
    }
### Sets the font color and fontsize within the content class for the p tag
    .content p {
        color: hsl(227, 10%, 46%);
        font-size: 13px;
    }
### Sets all the element in the footer class to flexbox, and adds space between them. Adds a top border thats 1px. Also adds a padding of 30px top\bottom and 50px left\right with a top margin of 30px
    .footer {
        display: flex;
        justify-content: space-between;
        border-top: 1px solid hsla(227, 10%, 46%, 0.2);
        padding: 30px 50px;
        margin-top: 30px;
    }
### sets the fontsize, font color, font weight (to bold) abd adds a 5px margin to the bottom
    .footer p.num {
        font-size: 18px;
        color: hsl(229, 23%, 23%);
        font-weight: 700;
        margin-bottom: 5px;
    }

#### the full css file
    css
    
    @import url('https://fonts.googleapis.com/css2?family=Kumbh+Sans:wght@400;700&display=swap');

    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    body {
        font-family: 'Kumbh Sans', sans-serif;
        background-color: hsl(185, 75%, 39%);
        display: flex;
        align-items: center; 
        min-height: 100vh;
        background-image: url('./img/bg-pattern-top.svg'), url('./img/bg-pattern-bottom.svg'); 
        background-repeat: no-repeat, no-repeat;
        background-position: right 48vw bottom 40vh, left 45vw top 44vh;
    }

    .container {
        margin: 0 auto;
        text-align: center;
    }

    .wrapper {
        max-width: 420px;
        background-color: #fff;
        border-radius: 15px;
        overflow: hidden;
        margin: 1rem;
    }

    .content img {
        width: 100px;
        height: 100px;
        border-radius: 50%;
        border: 4px solid #fff;
        margin-top: -52px;
        margin-bottom: 20px;
    }

    .content h2 {
        color: hsl(229, 23%, 23%);
        font-size: 18px;
        font-weight: 700;
        margin-bottom: 10px;
    }

    .content h2 span {
        color: hsl(227, 10%, 46%);
        font-weight: 400;
    }

    .content p {
        color: hsl(227, 10%, 46%);
        font-size: 13px;
    }

    .footer {
        display: flex;
        justify-content: space-between;
        border-top: 1px solid hsla(227, 10%, 46%, 0.2);
        padding: 30px 50px;
        margin-top: 30px;
    }

    .footer p.num {
        font-size: 18px;
        color: hsl(229, 23%, 23%);
        font-weight: 700;
        margin-bottom: 5px;

    }
# HTML

