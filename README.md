# MTLHateCorpus 2023
## Multi-task Learning for Hate Speech Detection: Identifying Speech Type, Target, Targeted-group, and Intensity in Spanish
https://www.sciencedirect.com/science/article/pii/S0920548925000194

The rise of digital communication has exacerbated the challenge of tackling harmful speech online, particularly hate speech, which dehumanises individuals or groups on the basis of traits such as race, gender or ethnicity. This study highlights the urgent need for fine-grained detection methods that take into account several subtasks of hate speech detection, including its intensity, determining the groups to which hate speech is directed, and whether the target is an individual or a group. Furthermore, there is a gap in comprehensive Spanish language datasets that cover these subtasks of hate speech detection. Therefore, we created a novel corpus entitled Spanish  to facilitate the analysis of hate speech in these subtasks and evaluated the effectiveness of the multi-task learning strategy using mBART, comparing its results with other Large Language Models using Zero-Shot Learning as a lower bound and Fine-Tuning as an upper bound. The results achieved by the Multi-Task Learning strategy demonstrated its potential to increase model versatility, allowing a single model to effectively tackle multiple tasks while achieving competitive results, particularly in target group recognition. However, the fine-tuning strategy still slightly outperform the Multi-Task Learning strategy in terms of macro F1-score. 

## Dataset
To request the dataset, please fill this form:

https://docs.google.com/forms/d/e/1FAIpQLSeqvkrt757WXvjSbtswQ3Uw6_wOmL3Mp-vddM3pDjBOPQw3Pg/viewform?usp=dialog

The statistics of the dataset are shown below:

| label                             | train | val  | test | total |
|-----------------------------------|-------|------|------|-------|
| hate                              | 8419  | 1804 | 1805 | 12028 |
| hope                              | 1840  | 395  | 395  | 2630  |
| none                              | 7545  | 1617 | 1617 | 10779 |
| offensive                         | 7025  | 1505 | 1506 | 10036 |
| total                             | 24829 | 5321 | 5323 | 35473 |

| label                             | train | val  | test | total |
|-----------------------------------|-------|------|------|-------|
| group                             | 7451  | 1588 | 1650 | 10689 |
| individual                        | 9852  | 2116 | 2062 | 14030 |
| none                              | 7526  | 1617 | 1611 | 10754 |
| total                             | 24829 | 5321 | 5323 | 35473 |

| label                             | train | val  | test | total |
|-----------------------------------|-------|------|------|-------|
| aporophobia                       | 498   | 90   | 121  | 709   |
| disablism                         | 158   | 39   | 34   | 231   |
| fatphobia                         | 4648  | 977  | 1008 | 6633  |
| homophoby                         | 11785 | 2536 | 2547 | 16868 |
| misogyny                          | 1360  | 280  | 290  | 1930  |
| profession                        | 940   | 212  | 200  | 1352  |
| racism                            | 4161  | 862  | 952  | 5975  |
| safe                              | 2130  | 458  | 424  | 3012  |
| transphoby                        | 4844  | 1067 | 1011 | 6922  |
| total                             | 30524 | 6521 | 6587 | 43632 |

| label                             | train | val  | test | total |
|-----------------------------------|-------|------|------|-------|
| 1-disagreement                    | 2305  | 470  | 505  | 3280  |
| 2-negative-actions-poor-treatment | 4408  | 882  | 915  | 6205  |
| 3-negative-character-insults      | 7151  | 1610 | 1582 | 10343 |
| 4-demonizing                      | 1168  | 266  | 222  | 1656  |
| 5-violence                        | 329   | 73   | 76   | 478   |
| 6-death                           | 87    | 9    | 17   | 113   |
| none                              | 9381  | 2011 | 2006 | 13398 |
| total                             | 24829 | 5321 | 5323 | 35473 |

## Citation
```
@article{pan2025spanish,
  title={Spanish MTLHateCorpus 2023: Multi-task learning for hate speech detection to identify speech type, target, target group and intensity},
  author={Pan, Ronghao and Garc{\'\i}a-D{\'\i}az, Jos{\'e} Antonio and Valencia-Garc{\'\i}a, Rafael},
  journal={Computer Standards \& Interfaces},
  volume={94},
  pages={103990},
  year={2025},
  publisher={Elsevier}
}
```

