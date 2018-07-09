
# Public Points


```python
# Getting the public point from a secret
from ecc import G

secret = 999
point = secret*G
print(point)
```

### Try it

#### Get the public point where the scalar is the following:
```
7, 1485, 2**128, 2**240+2**31
```


```python
from ecc import G

secrets = (7, 1485, 2**128, 2**240+2**31)

# iterate over secrets
for secret in secrets:
    # get the public point
    print(secret*G)
```
