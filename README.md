# Dataset Description for the three-dimensional bin packing (3DBPP)

This dataset serves as a valuable resource for conducting experiments and research in the field of three-dimensional bin packing.
The original data were collected from a local shipping company and consist of 20 different item sizes. The dimensions of each container are fixed, with a depth (D) of 587, width (W) of 233, and height (H) of 220. The format of this dataset aligns with the industry benchmark for this domain.
To expand the dataset, a simulation scenario was designed. In this scenario, the types of items to be processed are denoted as 'm', and the total number of items in each packing instance is denoted as 'n'. Multiple settings of 'm' and 'n' were used to create a set containing 100 instances, generated randomly based on quantity proportion probabilities. The format of these instance sets remains consistent with the established benchmark for three-dimensional bin packing.
For the 'm' and 'n' values, the following sets were defined: 'm = [3, 5, 8, 10, 12, 15, 20]' and 'n = [50, 100, 200]'. The corresponding sets of random instances, denoted as 'RIS(m, n)', were constructed accordingly.
Data instance files are named following the format 'rism_n'. In each instance set, the first line indicates the number of instances contained within that set, and the instances themselves are listed successively starting from the second line. As illustrated below, the first row of each instance signifies the quantity of generated instances in the set (instances are considered regardless of order). The second column specifies the dimensions of the container used. The third line provides information about 'm' (the type) and 'n' (the total number) of items to be processed within that instance. Subsequent sequences detail the depth, width, height, and quantity of each item type.
The following uses file ris3_50 as an example：
100 # number of instances contained in the instance set
1 # indicates the instance number
587 233 220 # container dimensions (D W H)
3 50 # item (n m)
1 120 100 108 22 # item parameters (S/N depth width height quantity)
2 120 80 74 20
3 120 80 39 8
