# Hello, people

I made this calculator project based on a tutorial on Youtube, and now i'm trying to learn new things to implement in this project, like key functions, bug fixing and other stuff...

You'll find two main files in this repository
  1. `index.html`
  2. `style.css`

The `index.html` setup is very simple, a main div, form input and a table to better organize the calculator buttons


I made in document Javascript in this project
Let's look at the code
```javascript
function equal(e) {
  if (e == "") {
    alert("Write an expression, please")
  } else {
    document.calc.textview.value = eval(document.calc.textview.value)
  }
}
```
This function was made for the equal button, i could simply put that in Inline Javascript at the element, but i wanted to make sure that the user actually put something to be calculated in the input textview, so the `if` statement stands for that, i passed the value of the textbox as an argument for the function, so, if it's empty an alert window will show up, case not, the expression will be calculated, as it should