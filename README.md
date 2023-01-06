# The problem

When you search on Google you have many results that pop up. But how does Google choose which pages should appear at the top of the results (considering they're not paid advertisments). Google needs to have the most credible and resourceful sources at the top of the page.

# NumericalComputation-GooglePageRank

This Python program implements the basic Page Rank algorithm that Google once used in it's founding days. 

# Implemntaion

There are many details to this algorithm which would take too long to explain, for more see (https://en.wikipedia.org/wiki/PageRank)

Although breifly, the key ideas of the algorithm can be explained:
* If many other web pages include links to your web page, then there must be a consensus that your web page is "important"
* Consider this analogy: you hear from your friends (other webpages) that a particular restaurant (a website) has great food. You trust your friend's opinion and thus that particular resturant must in fact have really good food.
* Overall, the more often your webpage is linked by other credible webpages, the higher your rank will be

Now, how do we translate this mathematically for the computer to solve?
* Nodes (circles) are websites!
* Arcs (arrows) represent links from one page to another

![image](https://user-images.githubusercontent.com/59632554/211064082-f78e8595-a612-46d9-a674-c225ab78943f.png)

We can then convert this data into a matrix and begin mutating the data to find each webpages Page Rank!

