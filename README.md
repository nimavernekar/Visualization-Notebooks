# Visualization Notebooks Repository

This repository contains Jupyter notebooks with visualizations, along with their corresponding HTML files for easy viewing.

**This is how it works:**

- 📓 We provide a structure in three parts.
- 🖼️ For each part, analyse relevant datasets and create a set of visualizations.



Each part contains a Jupyter Notebook (`.ipynb`) and an HTML export for viewing without running the code.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/Visualization-Notebooks.git
2. Navigate into a specific part folder and open the notebook:
  ```bash
  cd Visualization-Notebooks/Part1
  jupyter notebook Part1.ipynb
```

# Visualization Portfolio 📓

This notebook provides the starting point for information visualization portfolio. 

# Datasets

To provide inspiration, here are some links where you can find interesting datasets to analyze in your portfolio:
- https://github.com/rfordatascience/tidytuesday 
- https://www.destatis.de/DE/Service/OpenData/_inhalt.html
- https://www.ons.gov.uk/census/planningforcensus2021/ukcensusdata
- https://ec.europa.eu/eurostat/
- https://www.kaggle.com/datasets
- https://data.fivethirtyeight.com/ 
- https://corgis-edu.github.io/corgis/csv/ 
- https://github.com/textmining-infopros/Curated-Datasets
- https://www.data-is-plural.com/ / https://docs.google.com/spreadsheets/d/1wZhPLMCHKJvwOkP4juclhjFgqIY8fQFMemwKL2c64vk


Feel free to use other data sources as well, including own datasets!



# Useful snippets

Here are a few code snippets that might come in handy. Feel free to extend this if you come across something that you think might be useful for others in the course! It is perfectly ok to share snippets like that, e.g. on e-Learning or our Discord server.


Merge/join dataframes in pandas.
```pd.merge(left=dataset, right=dataset2, on='column name', how='left' etc.)```

Reoder categorical levels (e.g. sth. like low, medium, high) in seaborn plots.
```sns.barplot(data=..., x=..., y=..., order=['low', 'medium', 'high'])```


# Setup

You'll need at least the following pakages. Feel free to add further packages you need.

Note: It's ok if you prefer to use another "base setup", e.g. another Python visualization package instead of seaborn.
```
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

# Suggestion: 
If you'd like your portfolio to use a consistent style (and if you want to use seaborn for this), it might be a good idea to define palettes and a context up front here:
```my_cat_palette = sns.color_palette('Set2')```
```my_cont_palette = sns.color_palette('Blues')```
You can switch palettes with: sns.set_palette(palette_object)

Note that some libraries might expect matplotlib colormap objects. Conversion is possible.

Set context to notebook (sets the basic scaling of fonts etc.):
```sns.set_context('notebook')```

```data_folder = './data/' ``` # adjust to your filesystem / setup, if you like
