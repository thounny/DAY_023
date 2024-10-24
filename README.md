# DAY_023 | Interactive GIF Slider with Animated Transitions

## Project Overview

For **DAY_023** of my daily code challenge series, I created an **interactive GIF slider** using **HTML**, **CSS**, **JavaScript**, and **GSAP**. The slider transitions smoothly between animated GIFs, with titles animating into view, creating a highly engaging and dynamic user experience. This project showcases an image slider/content carousel built from scratch, featuring **stunning animations** powered by GSAP.

---
### Inspiration from Awwwards Element by Meetings
Check the site out here! [Meetings](https://www.meetings.fr/)

---

## Preview

![DAY_023 Preview](./assets/DAY_023_1.gif)

## Inspiration

![Meetings](./assets/DAY_023_2.gif)

---

## Key Features

- **Image Slider / Content Carousel**: Built from scratch using **HTML**, **CSS**, and **JavaScript**, the slider dynamically displays various content (GIFs and titles) with smooth transitions.
- **GIF Transitions**: Each slide showcases a different GIF, creating visually dynamic transitions between the content.
- **GSAP Animations**: The transitions between slides and titles are powered by **GSAP** for stunning animations and interactive experiences.
- **Custom Title Animations**: Each title animates into view with a staggered letter-by-letter effect, adding depth to the user interaction.

---

## GSAP in Action

### Title Animation

```javascript
gsap.fromTo(
  newTitle.querySelectorAll("span"),
  { y: 60 },
  { y: 0, duration: 1.25, stagger: 0.02, ease: "hop" }
);
```

Each letter of the title animates from below, creating a dynamic reveal as the new slide comes into view.

### Slide Transition

```javascript
gsap.to(slide, { ...props, duration: 2, ease: "hop" });
gsap.to(slide.querySelector(".slide-img"), {
  rotation: -props.rotation,
  duration: 2,
  ease: "hop",
});
```

Slides animate by rotating and transitioning smoothly into position, offering an engaging and fluid experience for the user.

---

## How to Run

1. **Clone the repository**:

   ```bash
   git clone https://github.com/thounny/DAY_023.git
   ```

2. **Navigate to the project directory**:

   ```bash
   cd DAY_023
   ```

3. **Open the `index.html` file** in your browser, or use a local development server like **Live Server** in VSCode.

---

## Project Structure

```bash
DAY_023/
|── assets/
|── fonts/
|── styles.css
|── script.js
|── index.html
```

---

## Technologies Used

- **HTML5**: For structure and layout.
- **CSS3**: To handle styling, layout, and animations.
- **JavaScript (ES6)**: For interactive functionality and slide control.
- **GSAP (GreenSock Animation Platform)**: Powers the smooth animations and transitions between slides.

---

## Author

![Logo](./assets/index_dwn.gif)

**Thounny Keo**  
Creative Developer & Designer  
Frontend Development Student | Year Up United

---

![miku](./assets/miku.gif)