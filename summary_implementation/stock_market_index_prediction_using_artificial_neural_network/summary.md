# Stock market index prediction using artificial nuerual network  
### Author
Amin Hedayati Moghaddam<sup>a</sup>, Moein Hedayati Moghaddam<sup>b</sup>, Morteza Esfandyari<sup>c</sup>  
- <sup>a</sup> Department of Chemical and Petroleum Engineering, Sharif University of Technology, Tehran, Iran
- <sup>b</sup> Faculty of Managing and Accounting, College of Farabi, University of Tehran, Qom, Iran
- <sup>c</sup> Department of Chemical Engineering, Faculty of Engineering, University of Bojnord, ,Bojnord, Iran  

### Journal
Journal of economics, finance and administrative science  
### Accpeted
1 July 2016  

---

### Abstarct
> In this study the ability of artificial neural network (ANN) in forecasting the daily NASDAQ stock exchange
rate was investigated. Several feed forward ANNs that were trained by the back propagation algorithm
have been assessed. The methodology used in this study considered the short-term historical stock prices
as well as the day of week as inputs. Daily stock exchange rates of NASDAQ from January 28, 2015 to
18 June, 2015 are used to develop a robust model. First 70 days (January 28 to March 7) are selected as
training dataset and the last 29 days are used for testing the model prediction ability. 
Networks for NASDAQ index prediction for two type of input dataset(four prior days and nine prior days) were developed
and validated.  

### Objective
Investigate the ability of ANN in forecasting the daily NASDAQ stock exchange rate.
Predicting NASDAQ index with several feed forward ANNs that were trained by the back propagation algorithm 
with the stort-term historical stock prices well as the day of week as inputs.  

### Hypothesis
Performance of predicting daily NASDAQ stock exchange rate with ANNs 
will be related to how many prior days of price data used as input.

### Methodology
The methodology considered the short-term historical stock prices as well as the day of week as inputs.  

1. **Equation**  

    **_y(k) = f(y(k-1),y(k-2),y(k-3), ...,y(k-n),D(k))_**   
    - **y(k)** : the stock price at time k.
    - **n** : the numberof historical days.
    - **D(k)** : the day of week.

2. **Dataset**  

    Daily stock exchange rates of NASDAQ from January 28, 2015 to 18 June, 2015.  
    - Train dataset : First 70 days (January 28 to March 7)
    - Test dataset : Last 29 days  
    
3. **Performance measure**  

    The determinant coefficient (**R<sup>2</sup>**) and the mean suqre error (**MSE**) of modeled otuput.  
    - **R<sup>2</sup>**
        
    - **MSE**
        
    










