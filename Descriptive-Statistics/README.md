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

Age, weight and salary are either intervals or ordinal data. So, we can use mean of median to 
 replace missing values of their data. 

![image](https://github.com/user-attachments/assets/89b60ab6-8f49-4b84-bdc3-6b5d99b98b02)

<br>

But since gender and degree are nominal / nominal + ordinal data, we cannot use either mean or median. We can replace the missing values with **mode** in this case. <br><br>

So, the measure of central tendency finds applications in EDA (Exploratory Data Analysis) and Feature Engineering.
<br><br>

---
