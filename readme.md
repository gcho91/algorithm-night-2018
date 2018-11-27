# Vestwell Whiteboarding Night

Below is a list of algorithmic problems to help you prepare for your next whiteboarding interview. They are categorized by difficulty level: beginner, intermediate and advanced. Choose a challenging one to push yourself! 

## Beginner 

1. **Is It A Palindrome?**

Write a function that takes in a string and returns true or false depending on whether or not that string is a palindrome.

Example: input 'racecar' -> true, input 'platypus' -> false

____

2. **@Me**

  Given an array of twitter handles, print a string that @s all the users.

  ex: ['Vestwell', 'GirlDevelopIt'] -> '@Vestwell @GirlDevelopIt'

____

3. **Build A Triangle**

 write a function that takes an integer, n, and prints out a triangle of base n to the console, ex:
```
        #

        ##

        ###

        ####

        #####

        ######

        #######

        ########
```
____

4. **Calculate genetics**

 Given the following object of parents and their genetic probabilities, write a function that takes two parents and two traits, and calculates the percent chance that a child with those parents will have that trait, based on the parents' genes _(note: for this question we are ignoring the dominant and recessive mechanisms of true gene expression)_


Ex: (['Amanda', 'Gerald'], ['blueEyes', 'brownHair']) -> .096% chance that their child will have both blue eyes and brown hair. 

```
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
    },

    Gerald: {
    
      eyes: {
    
      blueEyes: .1,
    
      brownEyes: .8,
    
      greenEyes: .1
    
        },
    
    hair: {
    
      blackHair: .2,
    
      brownHair: .8,
    
      blondeHair: 0,
    
      redHair: 0
    
        }
    
    },
    
    Marilyn: {
    
      eyes: {
    
      blueEyes: .6,
    
      brownEyes: .1,
    
      greenEyes: .4
    
    },
    
    hair: {
    
      blackHair: .9,
    
      brownHair: .1,
    
      blondeHair: 0,
    
      redHair: 0
    
        }
    
    },
    
    John: {
    
      eyes: {
    
      blueEyes: .1,
    
      brownEyes: .1,
    
      greenEyes: .8
    
        },
    
    hair: {
    
      blackHair: 0,
    
      brownHair: .1,
    
      blondeHair: .6,
    
      redHair: .3
    
        }
    },
    Ray: {
    
      eyes: {
    
      blueEyes: .1,
    
      brownEyes: .7,
    
      greenEyes: .2
        },
    hair: {
     
      blackHair: .4,
     
      brownHair: .3,
     
      blondeHair: .1,
     
      redHair: .2
     
    }

    },
    
    Roseanne: {
     
     eyes: {
     
      blueEyes: 0,
     
      brownEyes: .8,
     
      greenEyes: .2
    
    },
    
    hair: {
    
      blackHair: .5,
    
      brownHair: .3,
    
      blondeHair: 0,
    
      redHair: .2
    
    }
    
    }
}
```
____
## Intermediate

1. **Character Repeats**

 Write a function that takes in two parameters: a paragraph of text and a letter, and returns the number of times that letter appears in the paragraph.

 Ex: ('Hello, this is a sentence', 'e') -> 4
____

 2. **Turn DNA into RNA**

 Write a function that takes a string of DNA and turns into a string of RNA. DNA is made of up As Ts Cs and Gs. RNA is made up of As, Us, Ts and Cs. As match with Us, Ts match with As, Gs -> Cs, Cs -> Gs. DNA is also read backwards to create RNA. 

 Ex: 'ATTGCGATCGATT' -> 'AAUCGAUCGCAAU'

____

 3. **Remove Duplicates**

 Write a function that removes duplicates from an array of numbers. 

 Ex: [2, 4, 7, 22, 4, 2, 7] -> [2, 3, 4, 7, 22]

____

 4. **All Except i**
 
 Given an array of integers, create a new array with the product of all the integers except for itself. 
```
 Ex: [1, 2, 3] => [6, 3, 2] 
```

____
 ## Advanced 

1. **Stock Market**

Write an function makeMoney that takes in an array of stock prices and returns the best profit you could have made from one purchase and one sale. The prices in the array are in the sequence in which they were purchased and can only be sold after it was purchased.

Input: makeMoney([22, 6, 5, 8, 11, 10])

Output: 6 (highest profit is from 11 - 5)

____

2. **Calculate pi using Monte Carlo simulation**
Pi can be calculated using a Monte Carlo approach.

 Monte Carlo methods are a broad class of computational algorithms that rely on repeated random sampling to obtain numerical results. The basic idea is using randomness to solve problems that might be deterministic in principle.

 *In essence, Monte Carlo simulations use random sampling to approximate or predict outcomes in the real world. In essence, you define a range of possible inputs, randomly choose inputs in that range, observe the outcome, lather, rinse, repeat, until your CPU catches on fire.*

Hint: throw lots of darts at a dartboard. 

Extra credit: use your favorite threading or distributed system toolkit to run in parallel.

____

3. **Road not taken**

Consider this situation. The top number of this triangle is 62. Below it are two numbers 03 and 44,
below that are three numbers and so forth. 

Let us consider the "paths" for this triangle where we traverse from the top number, 62, to any bottom number
 while obeying this one rule:
        From any number we can go one of two places: either go straight down to the number below it, or down one and to the right one (to the number diagonally bottom-right)
         but NOT diagonally to the bottom-left.

Let us define the "score" of a path to be the sum of all the numbers on that path.

  1. What is the maximum "score" for the paths on this triangle?
  2. What is the 2nd-highest "score" for the paths on this triangle?

```
62
03 44
75 44 33
93 42 04 35
43 49 23 24 46
74 98 22 35 88 64
42 20 59 46 10 62 34
33 71 63 19 00 85 87 83
67 35 28 54 30 61 45 06 49
94 53 36 93 54 30 27 16 90 68
37 88 70 67 35 37 68 45 56 51 53
16 65 36 11 99 51 87 85 11 49 20 84
81 72 85 57 37 86 79 23 43 24 52 58 41
24 53 72 41 22 53 98 16 13 51 20 39 78 86
62 90 09 94 73 35 62 02 30 87 33 99 08 31 49
25 79 11 23 66 86 54 62 14 13 94 75 20 25 84 49
85 93 98 94 58 58 00 88 05 92 45 93 10 73 60 09 94
47 02 62 73 26 33 73 96 28 72 75 24 95 09 40 98 95 21
65 14 62 95 58 56 59 53 49 58 14 88 24 54 76 17 91 34 70
21 61 04 25 10 45 90 48 92 23 85 55 28 11 60 48 45 15 61 43
83 29 44 04 11 69 68 32 49 29 01 64 54 83 66 60 85 61 10 46 09
90 60 10 98 98 30 24 85 11 30 06 96 57 51 69 11 08 95 70 55 73 25
56 21 92 40 19 41 00 66 77 04 45 48 31 03 72 06 92 04 39 63 12 12 77
47 63 61 51 27 46 61 93 37 11 07 75 71 24 21 26 10 10 90 34 68 36 80 25
40 85 02 82 80 71 83 38 27 39 20 70 85 89 29 78 35 16 71 92 89 75 02 98 50
98 09 04 29 91 42 07 17 81 18 05 54 43 52 88 85 94 97 29 45 25 85 24 17 16 39
59 52 67 80 67 56 76 53 59 65 48 21 94 33 51 59 92 45 22 70 06 77 83 11 82 39 97
08 92 14 08 31 95 22 66 66 30 10 91 36 88 72 96 82 18 82 11 58 01 84 34 30 70 29 51
68 40 10 26 13 36 38 12 03 96 63 48 76 19 92 17 80 05 46 91 48 36 52 72 79 77 61 84 90
87 07 13 82 21 57 26 39 19 61 11 92 32 45 21 86 18 86 28 61 86 26 84 05 83 26 32 10 71 98
89 38 33 66 42 87 47 90 84 11 18 32 00 50 88 26 93 98 49 78 69 01 76 93 53 21 10 34 27 18 26
03 51 85 15 98 86 40 88 28 37 40 08 24 95 45 08 79 21 51 34 06 61 64 25 57 82 85 89 16 72 62 66
93 90 26 87 07 55 42 40 23 64 23 29 73 12 86 89 61 46 71 46 68 75 35 96 09 65 06 37 29 99 11 70 20
98 26 44 98 32 08 46 81 19 21 81 71 21 02 70 45 74 46 36 44 20 38 16 88 43 59 74 24 71 63 11 80 57 76
35 42 68 30 15 94 23 10 78 77 81 18 53 51 37 72 63 35 29 42 10 74 17 25 51 27 20 97 38 93 49 62 51 31 85
55 70 40 26 07 45 58 92 83 94 06 65 07 30 07 21 71 34 73 29 35 08 59 46 10 40 16 08 89 16 37 53 02 27 87 07
74 67 68 14 96 70 81 37 41 32 31 54 73 34 82 13 86 60 21 89 30 93 40 23 21 86 95 99 20 52 28 92 51 90 78 34 07
75 07 53 59 54 04 77 22 03 43 85 99 70 14 61 72 95 52 05 97 91 06 54 37 77 51 75 96 57 31 83 04 84 28 07 43 03 62
01 31 76 88 10 86 97 40 00 57 26 65 89 76 71 41 34 17 30 41 44 47 73 57 35 03 34 25 57 98 34 52 91 00 09 15 42 16 53
15 57 05 59 89 81 77 51 34 06 57 40 43 52 22 71 54 32 13 90 17 64 97 98 93 38 03 22 62 12 69 45 66 08 22 33 15 98 61 99
18 33 71 00 65 33 21 44 95 70 74 55 92 56 15 58 76 51 35 28 96 82 78 40 27 38 27 39 79 89 67 12 59 25 13 65 81 92 74 30 83
73 97 08 72 96 37 53 02 91 01 02 29 51 20 80 80 29 31 09 41 78 83 51 49 62 18 83 78 14 48 91 93 29 12 87 63 80 50 35 34 46 25
62 34 58 42 68 39 63 75 94 98 13 60 17 11 36 39 23 90 21 85 37 01 53 24 51 41 36 37 98 06 04 57 07 21 19 58 75 38 75 96 42 08 97
37 97 37 20 45 01 69 84 54 02 72 51 21 85 30 42 83 94 33 84 11 13 53 22 13 60 80 65 90 57 50 53 39 40 46 12 20 33 12 41 57 54 93 88
12 03 54 79 40 22 38 31 39 11 17 15 39 03 62 19 28 73 55 74 27 26 22 05 66 03 41 93 83 26 68 85 32 17 13 53 14 39 53 94 20 18 25 88 64
57 73 05 88 52 27 84 73 62 12 40 92 48 67 98 59 16 25 58 06 56 44 29 50 05 98 29 38 81 19 47 49 08 98 22 10 06 83 15 42 79 71 61 88 42 85
76 29 92 57 83 73 18 75 43 79 17 19 81 41 40 21 97 33 55 30 67 18 07 35 29 33 27 92 04 39 75 18 83 37 56 64 82 35 82 43 21 98 42 13 84 85 64
25 22 86 74 41 44 85 17 56 82 97 41 31 99 75 55 23 86 60 78 84 62 07 41 38 87 72 03 63 52 99 29 84 87 85 73 08 28 70 12 63 45 41 11 16 50 43 53
35 12 87 47 07 16 54 66 87 39 11 51 35 33 87 00 08 91 60 56 77 84 63 18 44 76 58 12 20 28 49 77 32 32 80 07 45 71 97 40 64 86 08 77 57 04 43 38 45
47 45 87 41 97 06 87 68 00 16 89 18 16 74 02 69 91 55 85 12 51 43 32 94 82 95 04 99 53 25 77 73 51 04 35 32 71 42 12 81 09 29 43 78 54 71 37 36 12 92
```


