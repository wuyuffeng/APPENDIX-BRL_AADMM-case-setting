# BRL_AADMM-case-setting
 The parameters and historical datasets of the case studies on energy sharing with 2, 10, 50 and 100 prosumers.

# Overview  
### This project is a instruction for the parameters and historical datasets of the case studies in our paper  _**"A Best Response Learning assisted Asynchronous ADMM for Real-Time Energy Sharing with Delay"**_.  
> _**2_Prosumers**_:The parameters and historical dataset of the case studies on energy sharing with 2 prosumers.  
> _**10_Prosumers**_:The parameters and historical dataset of the case studies on energy sharing with 10 prosumers.  
> _**50_Prosumers**_:The parameters and historical dataset of the case studies on energy sharing with 50 prosumers.  
> _**100_Prosumers**_:The parameters and historical dataset of the case studies on energy sharing with 100 prosumers.
# Requirements
>Python 3  
>Numpy  
# Opening method
### Take _**2_Prosumers**_ as an example, there are two type files. The _**Decision_Making_Model_Parameters.npy**_ is the parameters of prosumers' decision-making model. The _**pr_data i.xlsx**_ contains the data obtained by historical successful communication (Randomly generated).

## Run the following code in Python to open the _**Decision_Making_Model_Parameters.npy**_.
```Python
import numpy as np
dict_ = np.load('Decision_Making_Model_Parameters.npy',allow_pickle = True).item()
```
# Parameters Description
### Our data is structured in the form of a dictionary, where the meaning of different key is explained as follows:  

>_**'Qi'**_ : It refers to the _**Q<sub>i</sub>**_ in formula (2a);  
>_**'di'**_ : It refers to the _**d<sub>i</sub>**_ in formula (2a);   
>_**'Ai'**_ : It refers to the coefficient matrix of _**x<sub>i,r</sub>**_ in the inequality of formula (2b);  
>_**'Bi'**_ : It refers to the boundary vector of _**x<sub>i,r</sub>**_ in the inequality of formula (2b);  
>_**'E'**_ : It refers to the coefficient matrix of _**x<sub>i,r</sub>**_ in the equality of formula (2b);  
>_**'Di'**_ : It refers to the _**D<sub>i</sub>**_ in formula (2b);  

# Historical dataset Description
### Our data is structured in the form of a dictionary, where the meaning of different key is explained as follows:  

>_**'E'**_ : It refers to the _**E**_ in formula (2c);  
>_**'Di'**_ : It refers to the _**D<sub>i</sub>**_ in formula (2c);  
>_**'Ai'**_ : It refers to the _**A<sub>i</sub>**_ in formula (2b);  
>_**'Bi'**_ : It refers to the _**B<sub>i</sub>**_ in formula (2b);  
>_**'Qi'**_ : It refers to the _**Q<sub>i</sub>**_ in formula (2a);  
>_**'di'**_ : It refers to the _**d<sub>i</sub>**_ in formula (2a);   
>_**'ci'**_ : It refers to the _**c<sub>i</sub>**_ in formula (2a);
