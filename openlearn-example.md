# OpenLearn Images


<section-start>
```python

from IPython.display import Image

import pandas
import sqlite3
conn = sqlite3.connect('openlearn.sqlite')
```
</section-start>


<section-live>
<variable-string>image_text</variable-string>
```python

pd.read_sql("SELECT * FROM xmlfigures WHERE caption LIKE '%{q}%' LIMIT 10".format(q=image_text), conn)
```
</section-live>
