#  Best Time to Buy and Sell Stock

## Explanation

Given an array of stock prices, where `prices[i]` represents the price of a stock on the `i`th day, the goal is to find the maximum profit that can be achieved by buying the stock on one day and selling it on a later day.

Only one transaction is allowed.

### Example

```text
Input:
prices = [7, 1, 5, 3, 6, 4]

Output:
5
```

The best choice is:

```text
Buy at: 1
Sell at: 6

Profit = 6 - 1 = 5
```

## Features

* Solves the problem using a single traversal of the array.
* Tracks the minimum stock price.
* Calculates the maximum possible profit.
* Uses constant extra space.
* Provides an efficient O(n) solution.
* Includes a `main()` method for testing.

## How It Works

The program maintains two variables:

```java
int minPrice = prices[0];
int maxProfit = 0;
```

### Step 1: Track Minimum Price

As the array is traversed, the program checks whether the current price is smaller than `minPrice`.

If it is smaller, `minPrice` is updated.

### Step 2: Calculate Profit

For every price, the program calculates:

```text
profit = current price - minimum price
```

### Step 3: Track Maximum Profit

If the calculated profit is greater than `maxProfit`, the program updates `maxProfit`.

### Step 4: Return Result

After processing the complete array, `maxProfit` contains the maximum possible profit.

## Technologies Used

* Java
* Arrays
* Loops
* Conditional statements
* Methods
* Classes

## Data Structures Used

### Array

The input stock prices are stored in an integer array:

```java
int[] prices
```

The array stores the stock price for each day.

No additional data structure is required.

## Methods Used

### `maxProfit()`

```java
public static int maxProfit(int[] prices)
```

This method calculates and returns the maximum profit.

**Parameter:**

* `prices` – Array containing stock prices.

**Return value:**

* Maximum profit that can be obtained.

### `main()`

```java
public static void main(String[] args)
```

The `main()` method creates the input array, calls `maxProfit()`, and displays the result.

## Program Flow

```text
Start
  ↓
Create prices array
  ↓
Set minimum price
  ↓
Set maximum profit to 0
  ↓
Traverse the array
  ↓
Is current price smaller?
  ↓
Update minimum price
  ↓
Calculate profit
  ↓
Is profit greater than maximum profit?
  ↓
Update maximum profit
  ↓
Return maximum profit
  ↓
End
```

## Time Complexity

The array is traversed only once.

```text
Time Complexity: O(n)
```

where `n` is the number of stock prices.

## Space Complexity

Only a few variables are used.

```text
Space Complexity: O(1)
```

## Sample Input

```text
prices = [7, 1, 5, 3, 6, 4]
```

## Sample Output

```text
Maximum Profit: 5
```

## Key Learning

This problem teaches how to find the best buying and selling points while traversing an array only once.

The important idea is to always keep track of the **lowest price seen so far** and calculate the profit using the current price.

## File Location

```text
Arrays/BestTimeToBuyAndSellStock.java
```

## Repository Structure

```text
leetcode-java/
│
├── README.md
│
└── Arrays/
    ├── TwoSum.java
    └── BestTimeToBuyAndSellStock.java
```
AUTHOR
V.HARINI
