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

```python
> person
Circle: High School, Google Inc
Name: Ph.D John L Chaorai
Tel: 099 299 9999, ...
Birthday: 02 12 1990 (27y)
Note: A guy that make me laugh all the times.
Don't Eat Chocolate
...

> person.fullname
"Ph.D John L Chaorai"
see also .prefix .name .surname .middlename

> person.name = "Christ"
> person.fullname
"Ph.D Christ L Chaorai"
see also .prefix .name .surname .middlename

> person.update()

```
