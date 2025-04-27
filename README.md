# pstat131-homework-2-solved
**TO GET THIS SOLUTION VISIT:** [PSTAT131 Homework 2 Solved](https://www.ankitcodinghub.com/product/pstat-131-homework-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;119128&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;PSTAT131 Homework 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Linear Regression

The age of an abalone is typically determined by cutting the shell open and counting the number of rings with a microscope. The purpose of this data set is to determine whether abalone age (number of rings + 1.5) can be accurately predicted using other, easier-to-obtain information about the abalone.

The full abalone data set is located in the data subdirectory. Read it into R using read_csv() . Take a moment to read through the codebook ( abalone_codebook.txt ) and familiarize yourself with the variable definitions.

Question 1

Your goal is to predict abalone age, which is calculated as the number of rings plus 1.5. Notice there currently is no age variable in the data set. Add age to the data set.

Assess and describe the distribution of age .

Hide

above, we can see that the age of abalone is not distributed evenly. The shape of the distribution is skewed to the left with a clear mode around age of 11, and most of abalone’s age are around 8 to 13 and there is an outlier at around 30.

Question 2

Split the abalone data into a training set and a testing set. Use stratified sampling. You should decide on appropriate percentages for splitting the data.

Remember that you’ll need to set a seed at the beginning of the document to reproduce your results.

## type longest_shell diameter height whole_weight shucked_weight

## 2 M 0.350 0.265 0.090 0.2255 0.0995

## 5 I 0.330 0.255 0.080 0.2050 0.0895

## 36 M 0.465 0.355 0.105 0.4795 0.2270

## 38 F 0.450 0.355 0.105 0.5225 0.2370

## 43 I 0.240 0.175 0.045 0.0700 0.0315

## 45 I 0.210 0.150 0.050 0.0420 0.0175

## viscera_weight shell_weight rings age

## 2 0.0485 0.070 7 8.5

## 5 0.0395 0.055 7 8.5

## 36 0.1240 0.125 8 9.5

## 38 0.1165 0.145 8 9.5

## 43 0.0235 0.020 5 6.5

## 45 0.0125 0.015 4 5.5

Hide

head(abalone_test)

## type longest_shell diameter height whole_weight shucked_weight

## 6 I 0.425 0.300 0.095 0.3515 0.1410

## 11 F 0.525 0.380 0.140 0.6065 0.1940

## 17 I 0.355 0.280 0.085 0.2905 0.0950

## 19 M 0.365 0.295 0.080 0.2555 0.0970

## 21 M 0.355 0.280 0.095 0.2455 0.0955

## 24 F 0.550 0.415 0.135 0.7635 0.3180

## viscera_weight shell_weight rings age

## 6 0.0775 0.120 8 9.5

## 11 0.1475 0.210 14 15.5

## 17 0.0395 0.115 7 8.5

## 19 0.0430 0.100 7 8.5

## 21 0.0620 0.075 11 12.5

## 24 0.2100 0.200 9 10.5

Question 3

Using the training data, create a recipe predicting the outcome variable, age , with all other predictor variables. Note that you should not include rings to predict age . Explain why you shouldn’t use rings to predict age .

Steps for your recipe:

1. dummy code any categorical predictors

2. create interactions between

type and shucked_weight , longest_shell and diameter ,

shucked_weight and shell_weight

3. center all predictors, and

Question 4

Create and store a linear regression object using the “lm” engine.

Hide

Question 5

Now:

1. set up an empty workflow,

2. add the model you created in Question 4, and

3. add the recipe that you created in Question 3.

Question 6

Use your fit() object to predict the age of a hypothetical female abalone with longest_shell = 0.50, diameter = 0.10, height = 0.30, whole_weight = 4, shucked_weight = 1, viscera_weight = 2, shell_weight = 1.

Question 7

Now you want to assess your model’s performance. To do this, use the yardstick package:

1. Create a metric set that includes R2, RMSE (root mean squared error), and MAE (mean absolute error).

2. Use predict() and bind_cols() to create a tibble of your model’s predicted values from the training data along with the actual observed ages (these are needed to assess your model’s performance).

3. Finally, apply your metric set to the tibble, report the results, and interpret the R2 value.

The R^2 represents how well the regression model fits the observed data. As the we getting rsq about 0.56, the model is not fitting the observed data well.

The root mean squared error is the standard deviation of the residuals (prediction errors), As we are predicting the age of abalone, about 2.13 of rmse is a bit to big as a prediction error.

mae: The mean absolute error indicates that the magnitude of difference between the prediction of an observation and the true value of that observation is about 1.53.
