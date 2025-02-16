# TABLE OF CONTENTS
- [Measure of central tendency](#measure-of-central-tendency)
- [Choosing appropriate measure of central tendency](#choosing-appropriate-measure-of-central-tendency)
- [Applications of measure of central tendency](#applications-of-measure-of-central-tendency)
- [Measure of dispersion](#measure-of-dispersion)
- [Why is sample variance divided by n-1](#why-is-sample-variance-divided-by-n-1)
- [Random variables](#random-variables)
- [Percentiles and Quartiles](#percentiles-and-quartiles)


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
Population variance is divided by N while sample variance is divided by n-1. This is called **Bessel correction**. <br>

![image](https://github.com/user-attachments/assets/c93d9002-89bd-4a60-bebd-26a0cc055bd0)

<br>
So, this correction reduces the gap between actual values of population and sample variance. Thereby we can provide better insights of population data from sample data. **This doesn't entirely solve the problem but reduces the gap between the values.**


