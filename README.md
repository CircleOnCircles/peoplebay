# peoplebay
a pythonic interface for google contact aka. people api

## Installation

## API Design

```python
from peoplebay import Bay

bay = Bay([oauth])

# universal search
people = bay.search("John")
people = bay.getall()

for person in people:
  print(person)

```
