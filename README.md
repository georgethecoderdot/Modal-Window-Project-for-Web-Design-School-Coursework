# Modal Window Display Project

This project focuses on creating an interactive modal window. It demonstrates proficiency in HTML, CSS, and JavaScript, with the purpose of displaying a modal window when a button is clicked, and closing it when the user clicks outside the modal or presses the escape key.

## Project Description

This project features a simple yet modern website layout with three buttons that each opens a modal window. Each modal window contains a close button and a body of text. The modal window appears over a semi-transparent overlay that covers the entire webpage.

## Technologies Used

- HTML5: For creating the basic structure of the webpage.
- CSS3: For styling and animations.
- JavaScript (ES6+): For creating interactivity, including opening and closing the modal window.
- Google Fonts: For importing the 'Roboto' font.

## Features

- **Modern Design:** The design of the webpage is modern and clean, making use of soft colors and smooth animations.
- **Responsive:** The webpage is responsive and adjusts for different screen sizes.
- **Interactive:** The webpage has interactivity; buttons can be clicked to open and close the modal window.
- **User-Friendly:** The user experience was considered during development. If a modal window is open, it can be closed by clicking outside the modal or by pressing the Escape key.

## Project Setup

To get the project up and running, follow these steps:

1. Clone this repository to your local machine.
2. Open the index.html file in a web browser.

## Code Example

Here's an example of the JavaScript function used to close the modal:

```javascript
const closeModal = () => {
  modal.classList.add("hidden");
  overlay.classList.add("hidden");
};

btnCloseModal.addEventListener("click", closeModal);
overlay.addEventListener("click", closeModal);

document.addEventListener("keydown", (e) => {
  if (e.key === "Escape" && !modal.classList.contains("hidden")) {
    closeModal();
  }
});
```

## License

This project is open source, feel free to use it for your own purposes.
