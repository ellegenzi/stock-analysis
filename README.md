# Stock Analysis

## Overview of Project

### Background and Purpose

Steve is a recent graduate and now has a finance degree. His parents are very proud and want to be his first clients. They are passionate about green energy and are particularly interested in one company, DAQO New Energy Corp. However, Steve is concerned about diversifying and wants to analyze other green energy stocks as well. The purpose of this project was to help Steve analyze green energy stocks and provide him with efficient code that will allow him to expand the dataset for analysis to include the entire stock market over the last few years.

## Results

### How does the stock performance compare between 2017 and 2018?

Overall, 2017 was a much better year in regards to stock performance. 11 out of 12 stocks had positive returns in 2017, while only 2 out of 12 stocks had positive returns in 2018.

**2017 Performance**

![2017_StockPerformance](https://user-images.githubusercontent.com/106830513/175429723-9abeb5da-082a-43ab-b8c2-51e5dccbd8f6.png)

**2018 Performance**

![2018_StockPerformance](https://user-images.githubusercontent.com/106830513/175429731-c53cddfa-beb8-46b2-bbf9-dd22493b3d67.png)

### How do the execution times compare between the original script and the refactored script?

For the 12 green energy stocks, the execution times between both are very quick (less than 1 second), but the refactored script is significantly faster, by about 7x. This difference is mainly because the refactored script only runs through the entire dataset once using the tickerIndex variable vs multiple times with the original script (see screenshots of execution times and code below). Since Steve is planning to compare the green energy stocks to the entire stock market, which is a much larger volume of data, that 7x faster will become a bigger difference in execution time compared to the original script.

**Execution Times Before Refactoring**

![2017_Original_Code](https://user-images.githubusercontent.com/106830513/175429772-b7ad99df-020c-4fc0-92fd-1ac29c6a9d7d.png)
![2018_Original_Code](https://user-images.githubusercontent.com/106830513/175429789-a22681f3-9c00-4946-be87-7af7d6694e76.png)

**Execution Times After Refactoring**

![VBA_Challenge_2017](https://user-images.githubusercontent.com/106830513/175429828-54c61324-d613-407e-abe3-0a6de9907aca.png)
![VBA_Challenge_2018](https://user-images.githubusercontent.com/106830513/175429846-2db9f40b-84b6-40e2-9a0a-63c31431ce2d.png)

**Original Script**

![OriginalCode](https://user-images.githubusercontent.com/106830513/175429871-526ed5a8-3509-4d82-b36e-045266bac58f.png)

**Refactored Script**

![RefactoredCode](https://user-images.githubusercontent.com/106830513/175429881-d33e34e8-7820-40b1-8472-1e2778e32c3d.png)

## Summary

### What are the advantages or disadvantages of refactoring code?

An advantage of refactored code is that it can run faster! If the code doesn't require running through as many lines of data looking for what it needs, it can make large data files run code more quickly. A disadvantage is that it takes more time (and subsequently money in a business setting) to read through the original code and figure out methods to make it more efficient and flexible for a changing dataset.

### How do these pros and cons apply to refactoring the original VBA script?

The original VBA script required the code to run through every line of data each time to find the value needed that corresponded with the correct ticker. With the refactored script, the tickerIndex was able to increase once the ticker changed and it could get the values needed through only one scan of the entire dataset, thus making it run faster. Even though the refactored script was faster and could adapt to additional data, it took more time to write.
