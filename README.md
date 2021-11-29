# IMQ (interactive mentalizing questionnaire)

For different versions of IMQ (haiyanwu3@gmail.com)

## English version 
### Option 1

Qualtrics and using R to calculate the scores


        #delete items 3 6 11 and 19
        IMQdata <- IMQdata %>% dplyr::mutate(IMQ_SO = 5-IMQ_4 + 5-IMQ_5 + 5-IMQ_7 + 5-IMQ_9 + 5-IMQ_10 + 5-IMQ_13)
        IMQdata <- IMQdata %>% dplyr::mutate(IMQ_SS = 5-IMQ_2 + 5-IMQ_14 + 5-IMQ_17 + 5-IMQ_18 + 5-IMQ_20 + 5-IMQ_21 + 5-IMQ_23 + 5-IMQ_24)
        IMQdata <- IMQdata %>% dplyr::mutate(IMQ_OS = IMQ_1 + IMQ_8 + IMQ_12 + IMQ_15 + IMQ_16 + IMQ_22)
        IMQdata <- IMQdata %>% dplyr::mutate(total_study1 = IMQ_SO + IMQ_SS + IMQ_OS)



### Option 2

Running Eprime and get the IMQ_SS, IMQ_SO, IMO_OS and total IMQ score automatically

IMQ_EN.ebs


## Chinese version
### Option 1

wenjuanxing(wjx.com) and using R to calculate the scores

IMQ_SO: 是自我推论他人心理状态的能力

IMQ_SS: 是社会交互中心理理论的元认知（自信程度）

IMQ_OS: 是对于他人不能推论自己心理状态的自信


### Option 2
Running Eprime and get the IMQ_SS, IMQ_SO, IMO_OS and total IMQ score automatically

IMQ_CN.ebs


## Japanese version 
### option 1

Qualtrics and using R to calculate the scores


### Option 2
Running Eprime and get the IMQ_SS, IMQ_SO, IMO_OS and total IMQ score automatically

IMQ_JP.ebs


## references
1. Wu, H., Fung, B. J., & mobbs, d. (2019, July 31). Mentalizing during social interaction: the development and validation of the interactive mentalizing questionnaire. https://doi.org/10.31234/osf.io/g2zm8
2. Wu, H., Liu, X., Hagan, C. C., & Mobbs, D. (2020). Mentalizing during social InterAction: A four component model. Cortex, 126, 242-252.
https://www.sciencedirect.com/science/article/pii/S0010945220300277

