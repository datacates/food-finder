# food-finder
the ELI5 version of an algorithm to decide which meal to eat for nerds that track their food and have a bunch of data to use

I tracked every meal I ate from ~Nov 2022 through ~Nov 2023 (date of release) and asked the app support to send me all of the data that I had stored (apparently not a common request?). They sent me block of JSON text that was thick enough for space travel, which I wrangled through iterators and logical statements into a simple algorithm.

the function, which didn't really need to be written as such, takes the macro targets (carb, protein, fat) in grams, plus the current balance in those values, and a list of iar fngredients as parameters. Based on the ingredients and super basic text parsing, the script will figure out which meals are viable based on 1) what ingredients are on hand and 2) whether eating that meal would fit the macros remaining. it ultimately returns 1 food choice that will minimize the calories remaining.

I calculated how many times each of the ingredients appears in my food data and considered many other complicated enhancements like weighting how frequently I eat the food against the macro values, as well as creating multiple meal suggestions together to minimize the macro variance closer to zero. in the end, however, I would never care to use those things and this was sufficiently far for my purposes!
