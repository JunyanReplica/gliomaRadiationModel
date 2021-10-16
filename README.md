# Here is the code and data for the manuscript

## "A multi-compartment model of glioma response to fractionated radiation therapy parameterized via time-resolved microscopy data" Junyan Liu,David A. Hormuth II, Jianchen Yang, Thomas E. Yankeelov

## The data is in the MATLAB file DATA9L and DATAC6

DATA9L.fitGlobal is the parameter fitting/calibration results.
DATA9L.data.training is the 75% of total data for calibration.
DATA9L.data.validation is the 25% of total data for validation.

The data is labeled as 'dXfYiZ'. This stands for:
The dose X (round to the nearest integer as noted below)
Fraction numbers Y
Data are collected every Z hours.

For example, d4f4i4 stands for four fractions of 4 Gy. The microscope takes image every 4 hours.

**Note: that each fraction in our experiment is 24 hours apart so there's no label for that**

**Also note: The name "d5f3/d7f3" actually means 5.3Gy and 6.7 Gy. The reason we name it as "d5" and "d7" simply because MATLAB field name can't contain the symbol '.'. If checking the actual code, we use 5.3 and 6.7 in the calculation.**

# Constants9L and ConstantsC6 include some constants from our previous study: Liu, J., Hormuth, D. A., Davis, T., Yang, J., McKenna, M. T., Jarrett, A. M., ... & Yankeelov, T. E. (2021). A time-resolved experimental–mathematical model for predicting the response of glioma cells to single-dose radiation therapy. Integrative Biology.

These are constants that assumes unchanged throughout the study

### The entry point of the code is "main.m"
