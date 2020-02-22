#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a) A has a big notation of 0(n), since the iteration while be done for some period as it comparesthe value of a to that of n\*3. The notation for the constant becomes negligible as the value of n increases. so 0(n) is more consequential.

b) B has a big notation of 0(n log n), this is because while there's a loop going on, the while condition cuts the looping at a point such that not all items in the list or range is searched through, 0(n log n) is more effective

c) C has a big notation of 0(n) as the recursive function only calls itself once and does only an action on each loop

## Exercise II

Considering the need to minimize both dropped and broken eggs, i'll make us of the binary search method to find floor f. Abinary search method would have a big notation of O(log(n)) as it halves the list at every search; it is fast and will reduce the number of dropped eggs from various floors.

#### Steps:

- # n-story building is already sorted.

  1, declare a constant named break = 0

- 2, Divide the number of floors by two. Grab that middle which we will call M floor and drop an egg.
- 3a, If it breaks, assign break to M, leave out M and above, divide the floor between M and ground floor by two and assign it to the new M.
- 3b, However if the egg didn't break, leave out M and bellow, divide the remaing floor by two and assign M to the new middle.
- 4, Repeat same process until the floor where the egg doesnt break after breaking in the very previous floor.
- 5, Then return break (Because thats the last point it broke ),thus broke and above is floor f and above..
