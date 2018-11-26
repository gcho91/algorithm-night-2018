# Vestwell Whiteboarding Night

Below is a list of algorithmic problems to help you prepare for your next whiteboarding interview. They are categorized by difficulty level: beginner, intermediate and advanced. Choose a challenging one to push yourself! 

## Beginner 

1. **Is It A Palindrome?**

Write a function that takes in a string and returns true or false depending on whether or not that string is a palindrome.

Example: input 'racecar' -> true, input 'platypus' -> false

2. **Build A Triangle**

 write a function that takes an integer, n, and prints out a triangle of base n to the console, ex:

        #

        
        ##

        ###

        ####

        #####

        ######

        #######

        ########

3. **@Me**

  Given an array of twitter handles, print a string that @s all the users.

  ex: ['Vestwell', 'GirlDevelopIt'] -> '@Vestwell @GirlDevelopIt'

4. **Calculate genetics**

 Given the following object of parents and their genetic probabilities, write a function that takes two parents and two traits, and calculates the percent chance that a child with those parents will have that trait, based on the parents' genes.


Ex: (['Amanda', 'Gerald'], ['blueEyes', 'brownHair']) -> .096% chance that their child will have both blue eyes and brown hair. 

const people = {
    Amanda: {
     eyes: {
      blueEyes: .2,
      brownEyes: .8,
      greenEyes: 0
        },
     hair: {
      blackHair: .4,
      brownHair: .3,
      blondeHair: .1,
      redHair: .2
        }
    }
    Gerald: {
      eyes: {
      blueEyes: .1,
      brownEyes: .8,
      greenEyes: .1
        },
    hair: {
      blackHair: .2,
      brownHair: .8
      blondeHair: 0,
      redHair: 0
        }
    }
    Marilyn: {
      eyes: {
      blueEyes: .6,
      brownEyes: .1,
      greenEyes: .4
        },
    hair: {
      blackHair: .9,
      brownHair: .1
      blondeHair: 0,
      redHair: 0
        }
    }
    John: {
      eyes: {
      blueEyes: .1,
      brownEyes: .1,
      greenEyes: .8
        },
    hair: {
      blackHair: 0,
      brownHair: .1
      blondeHair: .6,
      redHair: .3
        }
    }
    Ray: {
      eyes: {
      blueEyes: .1,
      brownEyes: .7,
      greenEyes: .2
        },
    hair: {
      blackHair: .4,
      brownHair: .3
      blondeHair: .1,
      redHair: .2
        }
    }
    Roseanne: {
     eyes: {
      blueEyes: 0,
      brownEyes: .8,
      greenEyes: .2
        },
    hair: {
      blackHair: .5,
      brownHair: .3
      blondeHair: 0,
      redHair: .2
        }
    }
}
## Intermediate

1. **Character Repeats**

 Write a function that takes in two parameters: a paragraph of text and a letter, and returns the number of times that letter appears in the paragraph.

 Ex: ('Hello, this is a sentence', 'e') -> 3

 2. **Turn DNA into RNA**

 Write a function that takes a string of DNA and turns into a string of RNA. DNA is made of up As Ts Cs and Gs. RNA is made up of As, Us, Ts and Cs. As match with Us, Ts match with As, Gs -> Cs, Cs -> Gs. DNA is also read backwards to create RNA. 

 Ex: 'ATTGCGATCGATT' -> 'AAUCGAUCGCAAU'

 3. **Remove Duplicates**
 
 Write a function that removes duplicates from an array of numbers. 

 Ex: [2, 4, 7, 22, 4, 2, 7] -> [2, 3, 4, 7, 22]

 4. **All Except i**
 
 Given an array of integers, create a new array with the product of all the integers except for itself. 

 Ex: [1, 2, 3] => [6, 3, 2] 

 ## Advanced 


