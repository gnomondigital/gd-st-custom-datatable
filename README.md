# gd-st-custom-datatable

`gd-st-custom-datatable` is a custom streamlit component showing a [glide data grid](https://grid.glideapps.com/).

|   arg name      |      description             |
| --------------- | ---------------------------- |
| id_column        | column of the id for actions |
| height          | frame height                 |
| editables       | list of editable columns     |
| hides           | list of hidden columns       |
| add_view_column | add a view column            |
| column_width    | dict of column widths        |

# Quick use

```
import pandas as pd
from gdstdatatable import gd_datatable

df=pd.DataFrame(data={'id': [1, 2], 'name': ["ryu", "ken"]})

gd_datatable(df, id_column="id")

```

# Development

In `gdstdatatable/frontend` run:

```
npm install
npm start
```

In root folder:

```
poetry install
poetry shell
streamlit run gdstdatatable/example.py
```