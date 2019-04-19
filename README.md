# BudgetApp

This is a budget app allowing you to input incomes and expenses. 

This was the biggest Javascript project I have completed so far and was a good introduction to a Model View Controller type of planning 
your app and programming it. 

In the code you will see its split into 3 parts:
  
  Budget Controller
  UI Controller
  Global App Controller
  
So by doing this I was able to seperate out the code into more managable and organised sections.

The budget controller handled more of the 'backend' side of things, such as handle all the data gathered from the inputs 
by storing them in objects such as the data object, which stored my data arrays for expenses and incomes. It also stored my functions 
to do with manipulating the budget such as addItem(), deleteItem(). I also created my Expense and Income constructors here to.

As all 3 sections of the app needed to be independent of eachother they were all created as private functions and called with an IIFE then I returned an object which stored my functions, allowing me 
to use them in different parts of the app. 

The UI controller was the section to do with adding and deleting elements from the frontend. Such as creating new elements and adding to 
the DOM. This was actually my first time using the insertAdjacentElement() method, however it wasn't taking in my 2nd parameter. I then 
changed the method to insertAdjacentHTML() which seemed to work correctly. I also kept things such as all the class names in an object 
then used the variables when using queryselector. This was so handy as now if those class names ever need to be changed for some reason
I can just change the class name in the variable and it will update across the entire app.

The Global App controller was the part that connected it all together. So by calling the functions from the other sections of my app
I was able to create eventhandlers which would then call these functions and update the app.

This was overall a pretty long project, I did follow along to a tutorial but I learn so much a long the way about programming. Putting
the knowledge I have learned into a real world project has helped grow my skills heaps.

In the future I will be adding to the app, I'm just not sure what features to add yet.

Thanks for reading!
