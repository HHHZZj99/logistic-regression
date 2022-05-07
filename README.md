# logistic-regression
> train<-data.frame(click=c(1,1,0,1,1),url_1=c(0,0,1,0,1),url_2=c(0,1,0,0,0),url_3=c(0,1,0,0,1),url_4=c(1,0,1,0,0),url_5=c(0,1,0,0,1))
> fit<-glm(click~url_1+url_2+url_3+url_4+url_5,data=train,family=binominal(logit))
Error in binominal(logit) : 没有"binominal"这个函数
>  fit<-glm(click~url_1+url_2+url_3+url_4+url_5,data=train,family=binomial(logit))
> view(fit)
Error in view(fit) : 没有"view"这个函数
> head(view)
Error in head(view) : 找不到对象'view'
> head(fit)
$coefficients
  (Intercept)         url_1         url_2         url_3         url_4 
 2.456607e+01 -4.913214e+01 -4.913214e+01  4.913214e+01 -5.242491e-08 
        url_5 
           NA 

$residuals
         1          2          3          4          5 
 0.9999995  0.9999995 -1.0000000  0.9999996  0.9999984 

$fitted.values
           1            2            3            4            5 
1.000000e+00 1.000000e+00 2.143345e-11 1.000000e+00 1.000000e+00 

$effects
  (Intercept)         url_1         url_2         url_3         url_4 
-2.515734e-04 -2.054090e-04  1.383525e-13  2.651819e-04  2.829539e-13 

$R
              (Intercept)         url_1         url_2         url_3
(Intercept) -1.706782e-05 -6.827133e-06 -3.413563e-06 -6.827129e-06
url_1        0.000000e+00  8.361492e-06 -2.787164e-06  1.393582e-06
url_2        0.000000e+00  0.000000e+00 -6.232286e-06 -6.232286e-06
url_3        0.000000e+00  0.000000e+00  0.000000e+00  5.397321e-06
url_4        0.000000e+00  0.000000e+00  0.000000e+00  0.000000e+00
url_5        0.000000e+00  0.000000e+00  0.000000e+00  0.000000e+00
                    url_4         url_5
(Intercept) -6.827129e-06 -6.827129e-06
url_1        1.393582e-06  1.393582e-06
url_2        3.116143e-06 -6.232286e-06
url_3       -5.397321e-06  5.397321e-06
url_4       -5.397318e-06  0.000000e+00
url_5        0.000000e+00  1.000000e+00

$rank
[1] 5

