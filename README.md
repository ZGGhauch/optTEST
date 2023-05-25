# Classical Test Functions for Optimization

## About
This Python package provides a comprehensive list of classical test functions used in the optimization literature. The test functions can used to benchmark the performing of different optimization algorithms. The functions included in this Python package can be grouped into single-objective optimization, multi-objective optimization, and constrained optimization.

Author: Ziad Ghauch

## Installation

**Method 1**

Using the setup.py file, navigate to the package directory, then type
```
python setup.py install
```

**Method 2**

Alternatively, you can install this package directly from the GitHub repository, following
```
pip install git+https://github.com/ZGGhauch/optTEST
```

**Method 3**

You can also download the compressed version of the package, using
```
wget git+https://github.com/ZGGhauch/optTEST/archive/master.zip
unzip master.zip
cd optTEST
```

**Testing**

To run a comprehensive unit testing scheme on each optimization function, execute the following code
```
python -m unittest unit_tests.py
```

## List of Function

This different test functions supported in this package as listed in this section, for single-objective, multi-objective, and constrained optimization. 

### Single-Objective Optimization

| Function   |      Method      |  Dimension | Global Min |  Support |
|----------|:-------------:|:-------------:|:-------------:|:-------------:|
| Rastrigin |  rastrigin_function() | n | f(0,...,0)=0 | x$_i \in$[-5.12,5.12] |
| Ackley |  ackley_function() | 2 | f(0,0)=0 | x,y$\in$[-5,5] |
| Sphere | sphere_function()  | n | f(0,...,0)=0 | x$_i \in$($-\infty$,$\infty$) |
| Rosenbrock |  rosenbrock_function() | n | f(1,...,1)=0 | x$_i \in$(-$\infty$,$\infty$) |
| Beale |  beale_function() | 2 | f(3,0.5)=0 | x,y$\in$[-4.5,4.5] |
| Goldstein-Price | goldstein_price_function() | 2 | f(0,-1)=3 | x,y$\in$[-2,2]  |
| Booth | booth_function()  | 2 | f(1,3)=0 | x,y$\in$[-10,10] |
| Bukin | bukin_function()  | 2 | f(-10,1)=0 | x$\in$[-15,-5]y$\in$[-3,3] |
| Matyas |  matyas_function() | 2 | f(0,0)=0 | x,y$\in$[-10,10] |
| Levi |  levi_function() | 2 | f(1,1)=0 | x,y$\in$[-10,10] |
| Himmelblau | himmelblaus_function()  | 2 | f(3,2)=0 | x,y$\in$[-5,5] |
| Three-hump-camel | three_hump_camel_function()  | 2 | f(0,0)=0 | x,y$\in$[-5,5]   |
| Easom |  easom_function() | 2 | f($\pi$,$\pi$)=-1 | x,y$\in$[-100,100] |
| Cross-in-tray | cross_in_tray_function()  | 2 | f(1.3,-1.3)=-2 | x,y$\in$[-10,10] |
| Eggholder |  eggholder_function() | 2 | f(512,404)=-959| x,y$\in$[-512,512] |
| Holder-table | holder_table_function()  | 2 | f(8.1,9.7)==19.2 | x,y$\in$[-10,10] |
| McCormik |  mccormik_function() | 2 | f(-0.5,-1.5)=-1.9 | x$\in$[-1.5,4]y$\in$[-3,4] |
| Schaffer No 2| schaffer_function_n2()  | 2 | f(0,0)=0 | x,y$\in$[-100,100] |
| Schaffer No 4 |  schaffer_function_n4() | 2 | f(0,1.2)=0.3 | x,y$\in$[-100,100] |
| Styblinski–Tang | styblinski_tang_function() | n | f(-2.9,..,-2.9) | x$_i \in$[-5,5] |


### Multi-Objective Optimization

| Function   |      Method      |  Dimension |  Support |
|----------|:-------------:|:-------------:|:-------------:|
| Binh-Corn | binh_corn_function() | 2 |   x$\in$[0,5]y$\in$[0,3]|
| Chankong-Haimes | chankong_haimes_function() | 2 |  x,y$\in$[-20,20]|
| Fonseca-Fleming | fonseca_fleming_function() | n |  x$_i \in$[-4,4]|
| Kursawe | kursawe_function() | 3 |  x$_i \in$[-5,5]|
| Schaffer No 1 | schaffer_function_n1() | 1 | x$\in$[-A,A] |
| Schaffer No 2 | schaffer_function_n2() | 1| x$\in$[-5,10] |
| Poloni | poloni_function() | 2 | x,y$\in$[-$\pi$,$\pi$] |
| Viennet | viennet_function() | 2 | x,y$\in$[-3,3]|
| Osyczka-Kundu | osyczka_kundu_function() | 2 | x$_1$,x$_2$,x$_6$ $\in$[0,10], x$_3$,x$_5$ $\in$[1,5],x$_4$$\in$[0,6] |

### Constrained Optimization

| Function   |      Method      |  Dimension | Global Min |  Support |
|----------|:-------------:|:-------------:|:-------------:|:-------------:|
| Rosenbrock (cubic) | rosenbrock_constrained_cubic_function() | 2 | f(1,1)=0 | x$\in$[-1.5,1.5]y$\in$[-0.5,2.5] |
| Rosenbrock (sphere) | rosenbrock_constrained_line_function() | 2 | f(1,1)=0 | x$\in$[-1.5,1.5]y$\in$[-1.5,1.5] |
| Mishra | mishra_bird_constrained_function() | 2 | f(-3.1,-1.6)=-106 | x$\in$[-10,0]y$\in$[-6.5,0] |
| Townsend | townsend_function() | 2 | f(2.0,1.2)=-2.0 | x$\in$[-2.25,2.25]y$\in$[-2.5,1.75] |
| Gomez-Levi| gomez_levi_function() | 2 | f(0.09,-0.7)=-1.0 | x$\in$[-1,0.75]y$\in$[-1,1] |
| Simionescu | simionescu_function() | 2 | f(0.8,0.8)=-0.0  | x,y$\in$[-1.25,1.25] |


## Reference

+ https://en.wikipedia.org/wiki/Test_functions_for_optimization