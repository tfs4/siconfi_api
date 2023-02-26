
## Installation


```bash
pip install git+https://github.com/tfs4/siconfi_api.git
```

Dependencies:

* `pandas>=2.25.1`
* `requests>=1.2.1`

## Using
* `get_fiscal()` 
* `get_budget()` 
* `get_annual_acc()`
* `get_info()` 

Utility functions:

`find_cod()` to get the id (`cod_ibge`) for each state or city

Datasets:

* `br_cods`

## Examples


```python
from siconfipy import get_fiscal, get_budget, br_cods


if __name__ == '__main__':
    data = get_fiscal(year=2020, period=1, cod=35)
    data.to_csv('data.csv')
```

