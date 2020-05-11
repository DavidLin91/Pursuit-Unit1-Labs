# Initialization Lab


## Project Option 1: Structs Review

Download the resources at the link below:

https://developer.apple.com/go/?id=app-dev-swift-student (Links to an external site.)


Open the folder titled "2 - Introduction to UIKit" then open the folder titled "3 - Structures".  Open the Playground there, and work through the exercises.


## Project Option 2: Classes and Inheritance

Open the folder titled "2 - Introduction to UIKit" then open the folder titled "4 - Classes and Inheritance".  Open the Playground there, and work through the exercises.


## BONUS: Actor mini-project

Complete each of the following exercises by creating a new Command Line App in Xcode.  Classes and structs allow us to separate out our code into multiple different files.  In you main.swift file, copy and paste the code at the link below.

 https://gist.github.com/benstone1/75ae3cf24c8cb2ade792b9c66e79ee5c



## Step 1

Create a new file and name it "Movie.swift".  Make sure to save it right below your main.swift file.


Inside of the Movie.swift file, create a class called Movie that has properties for name (String), year (Int), genre (String), cast ([String]), and description (String).


Inside of main.swift, populate an array of Movies converted from the array of dictionaries in the gist above.

## Step 2

Then, for each movie in the Movie array, print the name of each movie and associated cast on a single line. Be sure not to print the array of cast members, only the string elements.



Correct Output Examples:

Minions: Sandra Bullock, Jon Hamm, Michael Keaton
Shrek: Mike Myers, Eddie Murphy, Cameron Diaz


Incorrect Output Examples (printing an array instead of the actors joined together as a String):

Minions: ["Sandra Bullock", "Jon Hamm", "Michael Keaton"]
Shrek: ["Mike Myers", "Eddie Murphy", "Cameron Diaz"]


## Step 3

Let's refactor our Movie class with what we learned today.



Create a failable convenience initializer convenience init?(with dict: [String:Any]) for the Movie class that takes in a dictionary, and uses the values of the input dictionary to initialize a Movie object.



Go back to the for loop in main.swift where we iterate through the movies array. Rewrite the body of the loop such that it creates a Movie object for each dictionary in the movies array using the new convenience initializer.


## Step 4

Repeating the same process you used to make the Movie.swift file, create files named:

- Person.swift
- Actor.swift


In Person.swift, create a class named Person with

- A name of type String
- A birthYear of type Int
- A deathYear of type Optional Int

In Actor.swift, create a class named Actor that

- Inherits from Person
- Has a breakoutYear of type Int
- Has a breakoutRole of type String

Rewrite your Movie class to have its case property be an array of Actors instead of Strings.

## Step 5

Repeating the same process you used to make the Movie.swift file, create a file named:

Genre.swift

In Genre.swift, create an enumeration with raw String values with the following cases:

- animation
- action
- drama


Rewrite your Movie class to have its genre property be of type Genre instead of String.


## Step 6

Refactor your code and create an area of your improved Movie class out of the array of dictionaries.

Then, use your new array to complete each of the following questions:

a. Print the name of the first movie.

b. Print a list of all movie names on one line.

c. Print a list of all movie years and names (each on a new line) as follows:

2015: Minions
2001: Shrek

d. Print the title of each movie and add an appropriate emoji to represent its genre.

e. Print out the title of each movie and all of the actors that were older than 40 when then movie was made.
