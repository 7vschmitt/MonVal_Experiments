
## Group 1

there are 30 answers for the test run which are a tillte bit different. The slider answer option "I don't want to pay for...", or "I don't want to sell..." are only integrated in the first 30 answers from the test run. 

For the rest of the 70 answers we shifted the answer options "I don't want to pay for...", or "I don't want to sell..."  to an additional carousel items, as too many participants just clicked on this option instead of using the slider. 

Please create one/or more variable(s), where you collect all the "I don't want to pay for...", or "I don't want to sell..." answers. The rest should be the same and you can simply merge the two data files. 

If you read in the json files and you want to flatten the list of answer you can simply use the following code: 


```
import json
import pandas as pd

df = pd.read_json("answers-group1-1.json")
data_sorted = df["formAnswers"].apply(pd.Series)
data_sorted 
```
