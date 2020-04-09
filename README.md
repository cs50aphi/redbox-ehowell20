# RedBox
You are probably familiar with the RedBox machines that you can see in Foodland, Safeway, and other public spaces. The RedBox machine allows you to rent and return DVDs to any location. In this problem, we will be simulating a virtual RedBox machine that will use an ArrayList to manage its list of DVD titles. It will also keep track of its inventory, and manage the user interface through a front-end menu-driven system. You’ll be completing all of the class files by implementing the methods that will perform a variety of operations that are sent in from the driver.

Go through the `RedBoxUI` driver, looking for the places where methods are called on the `RedBoxMachine` class that you will be writing. You will need to complete the methods in `RedBoxMachine` and `DVD` before you can finish the work in `RedBoxUI`.

`DVD.java` keeps track of the title of the movie, as well as the number of available copies of that movie so note that you will only have one DVD object for each title in the RedBox (even if there are many, many copies of Mall Cop 2.) Here's what you must do to complete `DVD.java`:

* Add instance variables
* Complete the constructor
* Write `incrementCopies()`
* Write `decrementCopies()`
* Write `getTitle()`
* Write `getNumCopies()`
* Write the `toString()` method

## RedBoxMachine
RedBoxMachine.java contains an instance variable that consists of an ArrayList that stores multiple instances of the `DVD` class. It also supports methods to search for available movies, and allows you to rent and return movies. It contains one method, `fillMachine()`, that has been completed for you. It loads the list of titles from MovieList.txt and adds them to the list of available movies by calling the `returnMovie()` method.

There's a lot of interrelated stuff in here so read carefully. The constructor relies on a pre-defined method called `fillMachine()` that fills the machine. The `fillMachine()` method in turn relies on `returnMovie()` which is one of the methods you need to write. So the constructor won't work until you write `returnMovie()`. Here's what you must do to complete `RedBoxMachine.java`:

*  Add instance variable
*  Write returnMovie()
*  Complete the constructor
*  Write getAvailableMovies()
*  Write rent()
*  Write searchForMovie()

## RedBoxUI
`RedBoxUI.java` contains the main method, and creates a new instance of the `RedBoxMachine` class. It uses `Scanner` to present the user with a list of prompts and allows the user to choose various functions that `RedBoxUI` then calls from the `RedBoxMachine` instance. Here's what you must do to complete `RedBoxMachine.java`:

*  Add code to display all available titles
*  Allow user to rent a movie, and display feedback
*  Allow user to return a movie, and display feedback
*  Allow user to search for a movie, and display feedback

As always, it is a good idea to check the documentation for the ArrayList class so you know how to add elements, remove elements, set elements, and get the size. As a tip, you may want to start with Googling "Javadocs ArrayList" and take a look at the class reference for ArrayList in the Javadocs documentation. Pay particular attention to the list of methods that ArrayList supports.

Think about how you might store the movies in a way that makes searching the ArrayList as efficient as possible.
