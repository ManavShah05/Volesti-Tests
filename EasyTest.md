# Easy Test
> Download, compile and run a simple sampling example with both C++ and R interfaces of volesti. For example, you can sample points from a 100-dimensional cube using the HMC algorithm implemented in volesti for various distributions.

### 1. C++ Interface

### Simple HMC Output:
[Output for C++ Interface](https://github.com/ManavShah05/VolestiTests/blob/main/outputs/OutputC.md)

### 2. R Interface:

### Code:
```
library(volesti)
P = gen_cube(100,'H')
pts = sample_points(P,100,NULL)
print(pts)
```

### Output:
[Output for R Interface](https://github.com/ManavShah05/VolestiTests/blob/main/outputs/OutputR.md)
