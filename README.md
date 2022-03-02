# IMQ (interactive mentalizing questionnaire)

For different versions of IMQ (haiyanwu3@gmail.com)

Using R to calculate the scores, notice that IMQ_SO and IMQ_SS are reverse scored:

        #delete items 3 6 11 and 19
        IMQdata <- IMQdata %>% dplyr::mutate(IMQ_SO = 5-IMQ_4 + 5-IMQ_5 + 5-IMQ_7 + 5-IMQ_9 + 5-IMQ_10 + 5-IMQ_13)
        IMQdata <- IMQdata %>% dplyr::mutate(IMQ_SS = 5-IMQ_2 + 5-IMQ_14 + 5-IMQ_17 + 5-IMQ_18 + 5-IMQ_20 + 5-IMQ_21 + 5-IMQ_23 + 5-IMQ_24)
        IMQdata <- IMQdata %>% dplyr::mutate(IMQ_OS = IMQ_1 + IMQ_8 + IMQ_12 + IMQ_15 + IMQ_16 + IMQ_22)
        IMQdata <- IMQdata %>% dplyr::mutate(total_study1 = IMQ_SO + IMQ_SS + IMQ_OS)

## English version 

Please see [here](https://github.com/andlab-um/IMQ/blob/main/IMQ_EN.docx).

## Chinese version

IMQ_SO: 是自我推论他人心理状态的能力

IMQ_SS: 是社会交互中心理理论的元认知（自信程度）

IMQ_OS: 是对于他人不能推论自己心理状态的自信

Please see [here](https://github.com/andlab-um/IMQ/blob/main/IMQ_CN.xlsx).

## References
1. Wu, H., Fung, B. J.s, & Mobbs, D. (2022). Mentalizing during social interaction: The development and validation of the interactive mentalizing questionnaire. Front. Psychol. 12:791835. https://www.frontiersin.org/articles/10.3389/fpsyg.2021.791835/full

2. Wu, H., Liu, X., Hagan, C. C., & Mobbs, D. (2020). Mentalizing during social interAction: A four component model. Cortex, 126, 242-252.
https://www.sciencedirect.com/science/article/pii/S0010945220300277

