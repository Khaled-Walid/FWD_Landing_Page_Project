# Landing Page Project

## Table of Contents

* [Usage](#Usage)
* [How it works](#how-it-works)

## Usage
[(Back to top)](#table-of-contents)

- Navigation among sections is possible through the navigation bar.
- Whenever the user stops scrolling, the navigation bar temporarily disappears until the user scrolls again.

## How it works
[(Back to top)](#table-of-contents)

1. Navigation bar is built by a function which loops over all sections, creates an anchor element inside an li element for each section, sets styling class for the li elements, sets an event listener for clicking on the li element and then appends all the created elements into the DOM.

2. Whenever an li element is clicked, it passes a click on the internal anchor element.

3. Intersection Observer API is used to build an observer to observe sections so that when a section is scrolled over, a class is added to that section to highlight it. It also highlights the related link element in the navigation bar.

4. Whenever the user scrolls, an event listener is triggered to keep showing the navigation bar. When the user stops scrolling, a timer is set to hide the navigation bar in 2 seconds.