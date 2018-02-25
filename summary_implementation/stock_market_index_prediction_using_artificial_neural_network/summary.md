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

    The overal procedure is governed by the following equation.  
    
    ![SMIPUANN_equ_3](https://github.com/aloefreshjihun/ai_finance_study/blob/master/summary_implementation/stock_market_index_prediction_using_artificial_neural_network/figure/SMIPUANN_equ_3.jpg)   
    - **y(k)** : the stock price at time k.
    - **n** : the numberof historical days.
    - **D(k)** : the day of week.

2. **Dataset**  

    Daily stock exchange rates of NASDAQ from January 28, 2015 to 18 June, 2015.  
    - Train dataset : First 70 days (January 28 to March 7)
    - Test dataset : Last 29 days  
    
3. **Performance measure**  

    The determinant coefficient (**R<sup>2</sup>**) and the mean suqre error (**MSE**) of modeled otuput were used to measure performance.  
    
    **R<sup>2</sup>**  
    ![SMIPUANN_equ_4](https://github.com/aloefreshjihun/ai_finance_study/blob/master/summary_implementation/stock_market_index_prediction_using_artificial_neural_network/figure/SMIPUANN_equ_4.jpg)  
    **MSE**  
    ![SMIPUANN_equ_4](https://github.com/aloefreshjihun/ai_finance_study/blob/master/summary_implementation/stock_market_index_prediction_using_artificial_neural_network/figure/SMIPUANN_equ_5.jpg)    
        
    - **y<sub>exp</sub>** : experimental values.
    - **y<sub>pred</sub>** : predicted vlaues.
    - **M** : the total number of data.
        
###  Experimental result  
Several networks for NASDAQ index prediction for two input dataset (four prior days and nine prior days) were developed and validated. Then the opimized network structure for both type of dataset was selected according to their abilities in prediction.

**Nomenclature**

|Abbreviation|Description|
|--|--|
|ANN|artificial neural networks|
|BPNN|back propagation neural network|
|MLP|multi-layer perceptron|
|LM|Levenberg-Marquardt|
|OSS|one step secant|
|GDA|gradient descent with adaptive learning rate|
|TANSIG||
|PURELIN||
|LOGSIG||

1. **For prior working days**  

    The values of R2 for different training algorithms and transfer function of a BPNN with 20-40-20 neurons in hidden layers have been tested.
    
    **Table 1.**   
    The prediction ability of a BPNN with 20-40-20 neruons and different training and transfer function.

    |No.|Training function|Transfer function|Train (R<sup>2</sup>)|Test (R<sup>2</sup>)|Validation (R<sup>2</sup>)|Total (R<sup>2</sup>)|
    |--|--|--|--|--|--|--|
    |1	|LM|	TANSIG	|0.9925|	0.9869|	0.8864|	0.974|
    |2	|LM|	PURELIN	|0.9457|	0.9675|	0.9027|	0.9395|
    |3	|LM|	LOGSIG	|0.9989|	0.9698|	0.7339|	0.9475|
    |4	|OSS|	LOGSIG	|0.9166|	0.9133|	0.8669|	0.9069|
    |5	|OSS|	PURELIN	|0.7016|	0.8824|	0.8230|	0.7675|
    |6	|**OSS**|	**TANSIG**	|**0.9386**|	**0.8917**|	**0.9408**|	**0.9267**|
    |7	|GDA|	LOGSIG	|0.9016|	0.8308|	0.8497|	0.8649|  
    
    **Table 2.**  
    The R<sup>2</sup> value for BPNN with different structure for four prior days
    
    |No.|Structure|Train (R<sup>2</sup>)|Test (R<sup>2</sup>)|Validation (R<sup>2</sup>)|Total (R<sup>2</sup>)|
    |--|--|--|--|--|--|
    |1	|2	|0.8177	|0.9616	|0.9493	|0.8692|
    |2	|5	|0.9250	|0.9188	|0.9605	|0.9264|
    |3	|5-5	|0.9229	|0.9724	|0.8631	|0.9212|
    |4	|5-10	|0.2185	|−0.0165	|−0.2065	|0.0838|
    |5	|10-10	|0.9534	|0.9602	|0.6811	|0.9344|
    |6	|10-20	|0.9059	|0.9758	|0.9108	|0.9263|
    |7	|40-40	|0.9003	|0.9639	|0.9616	|0.9264|
    |8	|50-100	|0.9576	|0.9324	|0.9393	|0.9483|
    |9	|100-200	|0.9390	|0.9466	|0.9533	|0.9393|
    |10	|200-300	|0.9267	|0.9642	|0.8822	|0.9276|
    |11	|20-40-20	|0.9386	|0.8917	|0.9408	|0.9267|
    |12	|20-50-20	|0.9403	|0.9417	|0.9077	|0.9374|
    |13	|50-100-50	|0.6837	|0.8108	|0.7785	|0.7326|
    |14	|20-40-40-20	|0.8990	|0.8445	|0.8093	|0.8739|
    |15	|10-20-20-10	|0.8977	|0.9602	|0.9015	|0.9109|
    |16	|10-20-20-20-10	|0.9304	|0.9341	|0.9456	|0.9329|
    
2. **Nine prior working days**  

    





