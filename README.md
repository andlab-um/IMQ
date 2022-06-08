# IMQ (interactive mentalizing questionnaire)

[![DOI](https://img.shields.io/badge/DOI-10.3389%2Ffpsyg.2021.791835-blue)](https://doi.org/10.3389/fpsyg.2021.791835)<br />
[![Twitter URL](https://img.shields.io/twitter/url?label=%40ANDlab3&style=social&url=https%3A%2F%2Ftwitter.com%2Flizhn7)](https://twitter.com/ANDlab3)
[![Twitter URL](https://img.shields.io/twitter/url?label=%40lizhn7&style=social&url=https%3A%2F%2Ftwitter.com%2Flizhn7)](https://twitter.com/lizhn7)

**For different versions of IMQ: <br />**
**Wu, H., Fung, B. J., & Mobbs, D. (2022). Mentalizing during social interaction: the development and validation of the interactive mentalizing questionnaire.** *Frontiers in psychology*, *12*. <br />
[DOI: 10.3389/fpsyg.2021.791835](https://doi.org/10.3389/fpsyg.2021.791835).

我们收到了不同单位的申请使用量表的邮件，

借此说明一下，我们的IMQ量表发表在OA期刊，正是为了方便大家的开放使用。

因此，在这一文件夹公布的问卷属于公开资源，不需询问申请，即可直接使用。

使用过程中有任何问题欢迎随时联系我（haiyanwu3@gmail.com）或ANDlab的博士生李肇宁（yc17319@umac.mo）。

感谢大家的关注！

We have been receiving emails from many teams asking for if they can use our scale. 

To clarify, our IMQ scale was published in OA journals precisely to facilitate open use.

In this case, the scale in this folder is an open resource that can be used without asking for our permission. 

If you encountered any problems while using this scale, feel free to email me (haiyanwu3@gmail.com) or Zhaoning Li, a Ph.D. student from ANDlab (yc17319@umac.mo).

Thanks for all the attention!

----
计分规则是：
Using R to calculate the scores, notice that IMQ_SO and IMQ_SS are reverse scored:

        IMQdata <- IMQdata %>% dplyr::mutate(IMQ_SO = 5-IMQ_3 + 5-IMQ_4 + 5-IMQ_5 + 5-IMQ_7 + 5-IMQ_8 + 5-IMQ_10)
        IMQdata <- IMQdata %>% dplyr::mutate(IMQ_SS = 5-IMQ_2 + 5-IMQ_11 + 5-IMQ_14 + 5-IMQ_15 + 5-IMQ_16 + 5-IMQ_17 + 5-IMQ_19 + 5-IMQ_20)
        IMQdata <- IMQdata %>% dplyr::mutate(IMQ_OS = IMQ_1 + IMQ_6 + IMQ_9 + IMQ_12 + IMQ_13 + IMQ_18)
        IMQdata <- IMQdata %>% dplyr::mutate(total_study1 = IMQ_SO + IMQ_SS + IMQ_OS)

## English version 

IMQ_SO, the ability to infer the mental states and thoughts of others

IMQ_SS, the ability to look inward to self-monitor and assess thought processes

IMQ_OS, the ability to make inferences about how much insight one think other agents have into one's own thoughts and intentions

Please see [here](https://github.com/andlab-um/IMQ/blob/main/IMQ_EN.xlsx) (excel) and [here](https://github.com/andlab-um/IMQ/blob/main/IMQ_EN.docx) (word).

## Chinese version

IMQ_SO: 是自我推论他人心理状态的能力

IMQ_SS: 是社会交互中心理理论的元认知（自信程度）

IMQ_OS: 是对于他人不能推论自己心理状态的自信

Please see [here](https://github.com/andlab-um/IMQ/blob/main/IMQ_CN.xlsx) (excel) and [here](https://github.com/andlab-um/IMQ/blob/main/IMQ_CN.docx) (word).

## Download link for the IMQ

- Baidu Netdisk: https://pan.baidu.com/s/1PryshD7nJ-5QArv-FVaHqA password: wdbh

## Following work

- [Every individual makes a difference: A trinity derived from linking individual brain morphometry, connectivity and mentalising ability](https://github.com/andlab-um/trinity)

## References
1. Wu, H., Fung, B. J.s, & Mobbs, D. (2022). Mentalizing during social interaction: The development and validation of the interactive mentalizing questionnaire. Front. Psychol. 12:791835. https://www.frontiersin.org/articles/10.3389/fpsyg.2021.791835/full

2. Wu, H., Liu, X., Hagan, C. C., & Mobbs, D. (2020). Mentalizing during social interAction: A four component model. Cortex, 126, 242-252.
https://www.sciencedirect.com/science/article/pii/S0010945220300277

## Bibtex citation

1.

    @article{Wu2022,
        author = {Wu, Haiyan and Fung, Bowen J and Mobbs, Dean},
        doi = {10.3389/fpsyg.2021.791835},
        journal = {Frontiers in Psychology},
        title = {{Mentalizing During Social Interaction: The Development and Validation of the Interactive Mentalizing Questionnaire}},
        volume = {12},
        year = {2022}
    }

2.

    @article{Wu2020,
        author = {Wu, Haiyan and Liu, Xun and Hagan, Cindy C. and Mobbs, Dean},
        doi = {10.1016/j.cortex.2019.12.031},
        journal = {Cortex},
        pages = {242--252},
        title = {{Mentalizing during social InterAction: A four component model}},
        volume = {126},
        year = {2020}
    }
