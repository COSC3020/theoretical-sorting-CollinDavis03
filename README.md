# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.
The way I would inspect this algorithm of a program is that this researcher is claiming that it runs this fast. With that runtime being _O_(n)
then no matter how many elements I put in the algorithm it should just be based on the inputs that are put into the algorithm. The inputs 
are n. The more inputs that I put in the runtime should increase linearly and not exponentially or stay the same. 

With that knowledge, I would put all different types of lists into the algorithm to see if it proves my theory. I would put three types of sorted lists
with a difference of 10 elements. This means one would be 10 elements for the next 20, and 30 for the last to see if it linearly increases with all the inputs. 
I would also add in reverse sorted lists, randomly sorted lists, and pattern lists. All those lists would follow the same guidelines as the sorted list. 
For the performance side of the algorithm, I would just give it massive lists and give it a list that would challenge the actual algorithm so that it will 
try to fight for the runtime analysis. If it follows that linear-based graph it will pass it. 

With all of that, I do not think that an algorithm can do this at all. It could do this between two elements. This just contradicts the lower bound of the comparison 
based on problems we have seen. The lower-bound comparison always performs Ω (n log n). With this, all the computations must perform this to get n. If it does not 
do this then it is not sorting at all. The conclusion is this is not possible at all. 
