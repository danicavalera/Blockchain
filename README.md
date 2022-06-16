# Blockchain

## Imports
```python
import streamlit as st
from dataclasses import dataclass
from typing import Any, List
import datetime as datetime
import pandas as pd
import hashlib
```

## Instructions
### Create a Record Data Class
Define a new Python data class named `Record`. Give this new class a formalized data structure that consists of the `sender`, `receiver`, and `amount` attributes. To do so, complete the following steps:
  * Define a new class named `Record`.
  * Add the `@dataclass` decorator immediately before the `Record` class definition.
  * Add an attribute named `sender` of type `str`.
  * Add an attribute named `receiver` of type `str`.
  * Add an attribute named `amount` of type `float`.

### Modify the Existing Block Data Class to Store Record Data

Rename the `data` attribute in your `Block` class to `record`, and then set it to use an instance of the new `Record` class that you created in the previous section. To do so, complete the following steps:
  * In the `Block` class, rename the `data` attribute to `record`.
  * Set the data type of the `record` attribute to `Record`.

### Add Relevant User Inputs to the Streamlit Interface

Code additional input areas for the user interface of your Streamlit application. Create these input areas to capture the sender, receiver, and amount for each transaction that you’ll store in the `Block` record.
To do so, complete the following steps:
  * Delete the `input_data` variable from the Streamlit interface.
  * Add an input area where you can get a value for `sender` from the user.
  * Add an input area where you can get a value for `receiver` from the user.
  * Add an input area where you can get a value for `amount` from the user.
  *As part of the Add Block button functionality, update `new_block` so that `Block` consists of an attribute named `record`, which is set equal to a `Record` that contains the `sender`, `receiver`, and `amount` values. The updated `Block`should also include the attributes for `creator_id` and `prev_hash`.

## Results
### The Pychain Ledger:
![Screen Shot 2022-06-15 at 5 17 21 PM](https://user-images.githubusercontent.com/97059769/173983744-c095a551-2f7f-47ab-b480-3531b7cd2534.png)

### Validation:
![Screen Shot 2022-06-15 at 4 50 37 PM](https://user-images.githubusercontent.com/97059769/173981962-9239cc0b-cee7-4e50-a690-202be3d60e9b.png)
![Screen Shot 2022-06-15 at 5 17 34 PM](https://user-images.githubusercontent.com/97059769/173983765-97eb10fe-2207-4ab3-abfb-c808a198233b.png)

