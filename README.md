# Three-Dimension Bin Packing Dataset

This dataset serves as a valuable resource for conducting experiments and research in the field of three-dimensional bin packing.

## Original Data Source 

The original data were collected from a local shipping company. It consists of 20 different item sizes and the dimensions of each container are fixed, with a depth (D) of 587, width (W) of 233, and height (H) of 220. The format of this dataset aligns with the industry benchmark for this domain.

## Dataset Description 

To expand the dataset, a simulation scenario was designed. In this scenario, the types of items to be processed are denoted as 'm', and the total number of items in each packing instance is denoted as 'n'. Multiple settings of 'm' and 'n' were used to create a set containing 100 instances, generated randomly based on quantity proportion probabilities. The format of these instance sets remains consistent with the established benchmark for three-dimensional bin packing.

For the 'm' and 'n' values, the following sets were defined: 'm = [3, 5, 8, 10, 12, 15, 20]' and 'n = [50, 100, 200]'. The corresponding sets of random instances, denoted as 'RIS(m, n)', were constructed accordingly.


## Dataset File Structure and Format

Data instance files are named following the format 'rism_n'. In each instance set, the first line indicates the number of instances contained within that set, and the instances themselves are listed successively starting from the second line. As illustrated below, the first row of each instance signifies the quantity of generated instances in the set (instances are considered regardless of order).The second line specifies the dimensions of the container used and the third line provides information about 'm' (the type) and 'n' (the total number) of items to be processed within that instance.Subsequent sequences detail the depth, width, height, and quantity of each item type.  

## Example: ris3_50

Let's take a look at an example using the file 'ris3_50':

- '100' indicates the number of instances contained in the instance set.
- '1' signifies the instance number.
- '587 233 220' represents the container dimensions (D, W, H) with depth, width, and height values.
- '3 50' denotes the item details (n, m), where 'n' is the total number and 'm' is the item type.
- '1 120 100 108 22' provides item parameters (S/N, depth, width, height, quantity) for the first item.
- '2 120 80 74 20' offers parameters for the second item.
- '3 120 80 39' provides parameters for the third item.

