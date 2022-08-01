# Frontend Mentor - Intro component with sign up form solution

This is a solution to the [Intro component with sign up form challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/intro-component-with-signup-form-5cf91bd49edda32581d28fd1). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page
- Receive an error message when the `form` is submitted if:
  - Any `input` field is empty. The message for this error should say *"[Field Name] cannot be empty"*
  - The email address is not formatted correctly (i.e. a correct email address should have this structure: `name@host.tld`). The message for this error should say *"Looks like this is not an email"*


### Links

- Solution URL: [Fronted Mentor Profile](https://www.frontendmentor.io/solutions/form-sign-up-with-validation-in-js-boostrap5-05CejY2Qzc)
- Live Site URL: [Netlify](statuesque-truffle-f7490a.netlify.app)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- Boostrap 5
- Javascript 
- [Font Awesome](https://https://fontawesome.com//) - For Icon

### What I learned

This is my first completed challenge, and I have learned the use of javascript to interact with hidden icons/img in the html:

```html
  <div class="wrapper">
    <input type="text" placeholder="First Name" id="Fname" name="Fname" class="inpt">
    <img src="images/icon-error.svg" alt="error-ico" id="Fname-ico" class="inpt-ico">
    <i class="fa-solid fa-circle-check inpt-ico-g" id="Fname-ico-g" ></i>
  </div>
```

```css
.wrapper{
  position: relative;
  width: 100%;
}

.inpt-ico-g, .inpt-ico {
  display: none;
  position: absolute;
  color: var(--green);
  font-size: 25px;
	width: 25px;
	height: 20px;
	right: 20px;
	top: 55%;
	transform: translateY(-50%);
}

.inpt-ico-active {
  display: block;
}
```

```js
if(validCondition){
  document.getElementById(`${id}-ico`).classList.add("inpt-ico-active");
} else {
  document.getElementById(`${id}-ico`).classList.remove("inpt-ico-active");
}
```


### Continued development

For my future developed projects I will use some backend language to save the information of the form in some database.

### Useful resources

- [Boostrap 5](https://getbootstrap.com/) - This helped me for add some fast sytle, i like to used in large projects.

## Author

- Personal Website - [Sandoval Ronald - Sodokun](https://github.com/Sodokun)
- Frontend Mentor - [@Sodokun](https://www.frontendmentor.io/profile/Sodokun)
