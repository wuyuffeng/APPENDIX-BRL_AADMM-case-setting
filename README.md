# APPENDIX & BRL_AADMM-case-setting

<div align="center">
  <img src = "title figure.png"/>
</div> 

# Overview  
This project is a instruction for the ***parameters*** and ***historical datasets*** of the case studies in our paper  ***"A Best Response Learning assisted Asynchronous ADMM for Real-Time Energy Sharing with Delay"***. Besides, the ***Appendix*** shown here, where the proofs of the Propositions are presented in detail.  

> _**2_Prosumers**_: The parameters and historical dataset of the case studies on energy sharing with 2 prosumers.  
> _**10_Prosumers**_: The parameters and historical dataset of the case studies on energy sharing with 10 prosumers.  
> _**50_Prosumers**_: The parameters and historical dataset of the case studies on energy sharing with 50 prosumers.  
> _**100_Prosumers**_: The parameters and historical dataset of the case studies on energy sharing with 100 prosumers.

# Requirements
>Python 3  
>Numpy  
# Opening method
Take _**2_Prosumers**_ as an example, there are two type files. <br>
The  ***"Decision_Making_Model_Parameters.npy"*** is the parameters of prosumers' decision-making model. <br>
The ***"pr_data i.xlsx"***" contains the data obtained by historical successful communication (Randomly generated).<br>

## Run the following code in Python to open the ***"Decision_Making_Model_Parameters.npy"***.
```Python
import numpy as np
dict_ = np.load('Decision_Making_Model_Parameters.npy',allow_pickle = True).item()
```
# Parameters Description
### Our parameters are structured in the form of a dictionary, where the meaning of different keys are explained as follows:  

>_**'Qi'**_ : It refers to the _**Q<sub>i</sub>**_ in formula (2a);  
>_**'di'**_ : It refers to the _**d<sub>i</sub>**_ in formula (2a);   
>_**'Ai'**_ : It refers to the coefficient matrix of _**x<sub>i,r</sub>**_ in the inequality of formula (2b);  
>_**'Bi'**_ : It refers to the boundary vector of _**x<sub>i,r</sub>**_ in the inequality of formula (2b);  
>_**'E'**_ : It refers to the coefficient matrix of _**x<sub>i,r</sub>**_ in the equality of formula (2b);  
>_**'Di'**_ : It refers to the _**D<sub>i</sub>**_ in formula (2b);  

# Historical dataset Description
### The historical dataset is recorded by .xlsx file, where the meaning of different columns is explained as follows:

>_**'Resource 1'**_ :  It refers to the upper boundary of Resource 1 in the successful communication data (the lower boundary defaults to 0);  
>_**'Resource 2'**_ :  It refers to the upper boundary of Resource 2 in the successful communication data (the lower boundary defaults to 0);    
>_**'Price'**_ :       It refers to the shadow price (or multiplier lamda) in the successful communication data;   
>_**'Demand'**_ :      It refers to the power demand (or _**D<sub>i</sub>**_) in the successful communication data;     
>_**'virtual_var'**_ : It refers to the auxiliary variable _**y<sub>i,sh</sub>**_ in the successful communication data;  
>_**'trade_volumn'**_ : It refers to the best response _**x<sub>i,sh</sub>**_ in the successful communication data;

# Appendix Description
### The ***Appendix.pdf*** records the proofs of Proposition 1 and Proposition 3~7 and 3 as follows:

>_**'Proposition 1'**_ : See (A1)-(A9) for details;  
>_**'Proposition 3'**_ : See (A10)-(A12) for details;  
>_**'Proposition 5'**_ : See (A13)-(A20) for details;  
>_**'Proposition 6'**_ : See (A21)-(A24) for details;  
>_**'Proposition 7'**_ : See (A25)-(A30) for details;  
>_**'Proposition 8'**_ : See (A31)-(A50) for details;  

