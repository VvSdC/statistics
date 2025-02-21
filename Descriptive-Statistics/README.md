# TABLE OF CONTENTS
- [Measure of central tendency](#measure-of-central-tendency)
- [Choosing appropriate measure of central tendency](#choosing-appropriate-measure-of-central-tendency)
- [Applications of measure of central tendency](#applications-of-measure-of-central-tendency)
- [Measure of dispersion](#measure-of-dispersion)
- [Why is sample variance divided by n-1](#why-is-sample-variance-divided-by-n-1)
- [Random variables](#random-variables)
- [Percentiles and Quartiles](#percentiles-and-quartiles)
- [5 number summary](#five-number-summary)
- [Histogram and Skewness](#histogram-and-skewness)
- [Covariance and Correlation](#covariance-and-correlation)

# Measure of central tendency

Measures of central tendency are statistical metrics that describe the center point or typical value of a dataset. They provide a single value that summarizes a set of data by identifying central position within that dataset.

Different measures of dataset:
- [Mean](#mean)
- [Median](#median)
- [Mode](#mode)

<br>

--- 

### Mean

Mean is the sum of all values divided by number of values.<br>

![image](https://github.com/user-attachments/assets/8eb45f14-120c-40fa-8c2a-5b30c9b53bee)

<br>

Characteristics of mean:
- [Mean is affected by extreme outliers](#affect-of-extreme-outliers-on-mean)
- Mean is used for interval and ratio data.

##### Affect of extreme outliers on mean:

![image](https://github.com/user-attachments/assets/5998ea2d-2211-495d-bcf1-613ae4169cae)

<br>
We can observe that adding just one outlier changed the mean from 3 to 22. So, we can say that mean can be affected by outliers. But **just because it is simply an outlier, we cannot remove it directly because every data point plays an important role**.
<br><br>

---

### Median

Median is the middle value in a dataset where values in the dataset are arranged in ascending or descending order.<br><br>

**If size of the data is odd** , Median is just the middle element of the dataset after arranging the data in ascending or descending order.

![image](https://github.com/user-attachments/assets/2276f93d-e99f-42ed-8485-d81dc4d32087)

<br>
**If size of the data is even**, Median is the average of two middle elements of the dataset after arranging the data in ascending or descending order.

![image](https://github.com/user-attachments/assets/e7016a5f-4226-4d6c-a0bd-c3c2132e1647)

<br>

Characteristics of median:
- [Median is not affected by extreme outliers](#affect-of-outliers-on-median)
- Median is used for ordinal,interval and ratio data.
<br>

##### Affect of outliers on Median

![image](https://github.com/user-attachments/assets/345db43a-ef75-4b3f-8b87-a68a2d150000)

We can see that addition of one outlier did not change the value of median. So, we can say that the median is immune to outliers.

<br><br>

---


### Mode

Mode is the value that occurs most frequently in a dataset.

![image](https://github.com/user-attachments/assets/c85cd563-81ef-4f02-9f31-dc98f5a6f199)

<br>

Characteristics of mode:
- Mode is not affected by outliers.
- This is used for all four scales of measurement of data i.e (Nominal scale, Ordinal scale, Interval scale and ratio scale). But this is often used for nominal scale.

<br><br>

---

# Choosing appropriate measure of central tendency

- **Mean**<br>
  Mean is best used when data is symmetrically distributed without any outliers. By providing 
  mathematical average, mean is useful for further statistical calculations.<br><br>
- **Median** <br>
  Median is best used when data is skewed or contains outliers. By providing middle value, 
  median better represents the center of skewed dataset. <br><br>
- **Mode** <br>
  Mode is best used for categorical data to identify most common category. It is useful for 
  identifying the most frequent value in ordinal, interval or ratio data.

<br><br>

---

# Applications of measure of central tendency

Suppose we have a dataset,

<table>
  <tr>
    <th>Age</th>
    <th>Weight</th>
    <th>Salary</th>
    <th>Gender</th>
    <th>Degree</th>
  </tr>
  <tr>
    <td>24</td>
    <td>70</td>
    <td>40k</td>
    <td>M</td>
    <td>BE</td>
  </tr>
  <tr>
    <td>25</td>
    <td>80</td>
    <td>70K</td>
    <td>F</td>
    <td>-</td>
  </tr>
  <tr>
    <td>27</td>
    <td>95</td>
    <td>45k</td>
    <td>F</td>
    <td>-</td>
  </tr>
  <tr>
    <td>24</td>
    <td>-</td>
    <td>50K</td>
    <td>-</td>
    <td>PhD</td>
  </tr>
  <tr>
    <td>32</td>
    <td>-</td>
    <td>60K</td>
    <td>-</td>
    <td>BE</td>
  </tr>
  <tr>
    <td>-</td>
    <td>60</td>
    <td>-</td>
    <td>-</td>
    <td>Masters</td>
  </tr>
  <tr>
    <td>-</td>
    <td>65</td>
    <td>55K</td>
    <td>M</td>
    <td>BSc</td>
  </tr>
</table>

<br>

Age, weight and salary are either interval or ratio data. So, we can use **mean or median** to 
 replace missing values of their data. 

![image](https://github.com/user-attachments/assets/89b60ab6-8f49-4b84-bdc3-6b5d99b98b02)

<br>

But since gender and degree are nominal / nominal + ordinal data, we cannot use either mean or median. We can replace the missing values with **mode** in this case. <br><br>

So, the measure of central tendency finds applications in EDA (Exploratory Data Analysis) and Feature Engineering.
<br><br>

---

# Measure of dispersion

Measures of dispersion describe the spread or variability of a dataset. They indicate how much the values in a dataset differ from the central tendency. <br>

Common measures of dispersion:
- [Range](#range)
- [Variance](#variance)
- [Standard Deviation](#standard-deviation)
- [Interquartile Range(IQR)](#interquartile-range)

<br><br>

---

### Range

Range is the difference between the maximum value and minimum value in a dataset.

![image](https://github.com/user-attachments/assets/b984182b-2599-417a-a75e-d62e27166055)

<br>

Characteristics of range:
- Simple to calculate.
- [Very sensitive to outliers](#affect-of-outliers-on-range)
- Just provides the rough measure of dispersion (because we care only about maximum and minimum values in the distribution and donot care about other values).

<br>

##### Affect of Outliers on Range

![image](https://github.com/user-attachments/assets/cc21b5e5-7a35-4196-beeb-251ebc005c7e)

Adding just one outlier changed the range drastically. So, range is very sensitive to outliers.

<br><br>

---

### Variance

Variance measures the average squared deviation of each value in the dataset from the mean. It provides a sense of how much the values in a dataset vary. <br>

Types of variance:
- [Population variance](#population-variance)
- [Sample variance](#sample-variance)

<br>

##### Population variance

![image](https://github.com/user-attachments/assets/dd90a8df-79f6-48da-b605-14a12f1a8849)

<br>

Example of population variance:

![image](https://github.com/user-attachments/assets/fac36401-5598-464a-ab2a-bcd22e9a8b9b)

<br><br>

##### Sample variance

![image](https://github.com/user-attachments/assets/e13b26aa-d0d3-426a-b588-a901a01a5be9)

**Population variance is divided by N while sample variance is divided by n-1 because of Bessel's correction**. Go to [why is sample variance divided by n-1](#why-is-sample-variance-divided-by-n-1) to understand. <br>

Characteristics of variance:
- Variance provides a precise measure of variability.
- Units of variance are squared of the original units
- [Very sensitive to outliers than the range](#affect-of-outliers-on-variance)
<br>

##### Affect of outliers on variance

![image](https://github.com/user-attachments/assets/32e561a7-564b-40e8-ab82-976945742e4e)

<br>

Adding an outlier changed the value of variance drastically. The change is more drastic compared to range. So, variance is more sensitive to outliers than the range. This is because we square up in variance.

<br><br>

---

### Standard deviation

The standard deviation is the square root of the variance. <br>

![image](https://github.com/user-attachments/assets/56008096-9602-4657-90c9-579cbf557579)

<br>
Identifying which data point falls under which standard deviation it falls from the mean, <br>

![image](https://github.com/user-attachments/assets/f7b210ad-07b3-48f0-922a-59e0dafb4fa2)

<br>

Characteristics of standard deviation:
- Provides a clear measure of spread in the same unit as the data.
- Standard deviation is sensitive to outliers. (Since it is just square root of variance which also is sensitive to outliers).

<br><br>

---

# Why is sample variance divided by n-1

![image](https://github.com/user-attachments/assets/c297a885-7178-423b-9d4f-5638e59cc148)

<br>
Population variance is divided by N while sample variance is divided by n-1. This is called **Bessel correction**.  It is done because if we donot select sample data properly from population data, we often underestimate the value of population variance. So, to avoid this we use this correction to increase the value of sample variance to bridge the gap between values of sample and population variance.
<br><br>

![image](https://github.com/user-attachments/assets/c93d9002-89bd-4a60-bebd-26a0cc055bd0)

<br>

So, this correction reduces the gap between actual values of population and sample variance. Thereby we can provide better insights of population data from sample data. **This doesn't entirely solve the problem but reduces the gap between the values**

<br><br>

---

# Random variables

Random variables is a function whose values are derived from different processes or experiments. <br>

Examples of random variables :
- Tossing a coin <br>
  X = { Head (0) or Tail (1) }
- Rolling a fair dice <br>
  X = {1 or 2 or 3 or 4 or 5 or 6}
<br>

Types of random variables : 
- [Discrete random variables](#discrete-random-variables)
- [Continuous random variables](#continuous-random-variables)
<br>

### Discrete random variables
Discrete random variables have countable number of outcomes and are typically whole numbers.<br>
Examples of discrete random variables:
 - Number of students in the class <br>
   Possible outcomes = 0 to maximum number of students in class and are integers
 - Number of heads obtained after tossing a coin thrice
   Possible outcomes = 0 to 3 and are integers
   <br>

### Continuous random variables
Continuous random variables can take any value within a given range, including decimals and fractions. <br>
Examples of continuous random variables:
- Height of a person <br>
  Possible outcomes = uncountable.
  Posssible values = {5.7ft, 5.756ft, 5.7556ft...}
- Time taken by a person to complete race
  Possible outcomes = uncountable and can be fractions/decimal numbers
  Possible values = {9.80s,9.8026s......}

  <br><br>

  ---

# Percentiles and Quartiles
- [Percentiles](#percentiles)
- [Quartiles](#quartiles)

### Percentiles

A percentile is a value below which certain percentage of observations lie.
<br>

![image](https://github.com/user-attachments/assets/11a76435-e25f-44c7-a9b9-0d7d307b6fb4)

<br>

Finding nth pecentile value,
<br>

![image](https://github.com/user-attachments/assets/4d4a952a-06b4-4ddd-b319-979f1d508f0e)

<br>

### Quartiles

Every 25th percentage of the distribution is a quartile. <br>

- 25th percentage -> 1st Quartile (Q1)
- 50th percentage -> 2nd Quartiles (Q2)
- 75th percentage -> 3rd Quartile (Q3)

<br><br>

---

# Five number summary

- Minimum
- 1st Quartile (Q1) -> 25th percentile
- Median
- 3rd Quartile (Q3) -> 75th percentile
- Maximum

To remove outliers, we define values of lower fence and higher fence. The values lesser than lower fence are outliers and the values greater than upper fence are also outliers. 

<br>

![image](https://github.com/user-attachments/assets/7d8bf3c0-1b25-436d-bff8-ee774196a612)

<br>

![image](https://github.com/user-attachments/assets/0eb54401-a7b8-4717-bcdb-29677d1a66ce)

<br>

![image](https://github.com/user-attachments/assets/b69e8bfa-2b1e-47af-88b3-a0916648754f)


<br><br>

---

# Histogram and skewness

A histogram is a physical representation of the distribution of numerical data. It is an estimate of the probability distribution of a continuous variable and is used to visualize shape,central tendency and variability in dataset.<br>

![image](https://github.com/user-attachments/assets/0b21613f-872a-4d51-b116-0ae4ff2b918f)

<br>

**Normal distribution :** <br>

![image](https://github.com/user-attachments/assets/a749a259-bd3c-43e6-b878-3ad6988c0c6c)

**Right skewed distribution:** <br>

![image](https://github.com/user-attachments/assets/17abc971-9edb-4eb5-9fb0-191083cd274a)

<br>

**Left skewed distribution :** <br>

![image](https://github.com/user-attachments/assets/4536192c-b8dc-4b62-b6d5-4b805e8c5992)

<br>

**Summary of skewness:** <br>

![image](https://github.com/user-attachments/assets/c8014497-1687-4643-a411-f13ce1417dcf)

<br><br>

---

# Covariance and Correlation

Covariance and correlation are two statistical measures used to determine the relationship between two variables. Both are used to understand how changes in one variable are associated with changes in another variable.

- [Covariance](#covariance)
- [Correlation](#correlation)

<br><br>

### Covariance

Covariance is a measure of how much two random variables change together. If the variables tend to increase and decrease together, the covariance is positive. If one tends to increase when the other decreases, the covariance is negative.

