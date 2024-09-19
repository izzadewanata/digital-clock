HTML
------------
    Write h2 -> heading
    Insert a div, with a class
        Insert 4 div -> in 3 of them, write 2 span element to host the figures with id (00) and host the text with class (hours). in the last div, create only 1 span with id for AM/PM.


CSS
------------
    body -> margin:0, content to the center of the page, flex-direction:column, backg photo:url("..."), background-size:cover, font-family

    h2 -> text-transform (Capital), letter-spacing, font-size, text-align, color

    .clock -> display:flex

    .clock div -> give margin

    .clock span -> display:flex, justify-content, align-items:center, width, height, background, opacity, color, font-size, text-shadow. Make this in large-size.

    .clock .text -> height, font-size, Uppercase, letter-spacing, background, opacity. Make this way smaller than the span

    Insert position:relative into -> .clock div

    .clock #ampm -> position:absolute, bottom:0, width, height (same with .text), font-size, backg:contrast


JavaScript
------------
    get hourEl, minuteEl, secondEl, ampmEl

    call the function.

    write a function to update the clock -> 
        declare h,m,s (with let) and give it a live time value: new Date().getHours()
        
        declare ampm and assign default value, "AM"

        write if condition for pm: hour minus 12 and set ampm to string "PM"

        assign h,m,s,ampm into Variables, using innerText

        write setTimeout method, to call the function every second (1000ms)
        
        maintain 2 digits on every div -> give h,m,s variable a conditional (ternary) operator, where if h is less than 10, then add "0" before h, otherwise the value is stay as it is