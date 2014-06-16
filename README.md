Function help
=============

**nanfillts**

  **nanfillts** Fill NaNs in the time series with the previous valid observation
 
    ```nanfillts(TSPANEL) TSPANEL should be a numeric matrix (or a vector) 
                       where each series is a column with the oldest 
                       observations in the first row (element) and the 
                       most recent ones in the last row (element).
 
    nanfillts(..., NOTRAIL) To avoid extrapolation of the last value of a 
                            time series till the end of the panel, set 
                            NOTRAIL to true (1). By default is false (0).
 
 
    TSPANEL = nanfillts(...) Returns the same matrix with filled NaNs.
 
    NOTE: leading NaNs are left untouched.
 
 
  Example:
 
    % Input data       % Simple call       % No trailing
                       nanfillts(ts)       nanfillts(ts,1)
     ts =              ans =               ans = 
         10  NaN            10  NaN             10  NaN
        NaN  NaN            10  NaN             10  NaN
        NaN    1            10    1             10    1
          9    2             9    2              9    2
        NaN  NaN             9    2            NaN  NaN
 
  
See also
interp1q
```
   
