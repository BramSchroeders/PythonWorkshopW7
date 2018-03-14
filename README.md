# Workshop Python 14/03

The main goal of this workshop is to familiarise yourself with Python and some of the most important modules it has to provide.
It's not important to gain a deep understanding in these modules, raising awareness of their existance and capabilities is key.

## Working environment and preliminaries

To achieve this goal, you will use Spyder. Spyder is an IDE for Python development. Open Spyder by pressing <kbd>⊞ Win</kbd> and typing 'Spyder'. Spyder's user interface is straightforward, the instructor will help you get started. There is no time for a basic introduction, please consult the cheatsheet.

## The beer data set
The dataset we will be using in this workshop is the beer data set. The description of this data is can be found [here](https://www.kaggle.com/c/beer-ratings/data "The beer data set").

## Access the data
[Pandas](https://pandas.pydata.org/ "Pandas website") is a data analysis module for Python. One of the features is accessing data.
Import pandas by using:
```python
import pandas as pd #as pd is optional but it's more practical to use aliases
```
Now use Pandas to read the CSV file in a [DataFrame](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.html).
<details><summary><b>Hint</b></summary>
<p>
  
```python
beer_data = pd.read_csv('path_to_your_csv_file.csv')
```

</p>
</details>


### Basic statistics






<details><summary>CLICK ME</summary>
<p>

#### yes, even hidden code blocks!

```python
print("hello world!")
```

</p>
</details>



```python
import numpy
```
