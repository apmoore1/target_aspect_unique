# Analysis of same aspect multiple times in a text and implicit targets.

This is done for my thesis. Link to the thesis will appear when it is avliable.

This is only to store the following [notebook](https://github.com/apmoore1/target_aspect_unique/blob/master/texts_contain_the_same_aspect_more_than_once.ipynb). The [notebook](https://github.com/apmoore1/target_aspect_unique/blob/master/texts_contain_the_same_aspect_more_than_once.ipynb) shows if the same aspect occurs in a text more than once for the SemEval 2015, and 2016 restaurant datasets. We are only going to look at sentences that contain (target, aspect, sentiment) where aspect can also be an (entity, aspect) pair. The reason why an aspect or (entity, aspect) pair can occur more than once in a text is because it is attached to a target that is within the text. Thus there could be the following case:

```
The CPU memory is great and so in the RAM
```

Given this text we could have the following annotations (memory, MEMORY, positive) and (RAM, MEMORY, positive) where the following represent (target, aspect, sentiment). Thus in this case the MEMORY aspect has occured twice in the same text. The reason we want to see if this occurs or not in the SemEval datasets is to see if we could treat the target sentiment problem as just a text/sentence level aspect based sentiment analysis task. Further whether when trying to identify aspects whether this has to be done at the target level or if it could be done at the text/sentence level.

Also we explore in the notebook how many samples are affected by implicit targets which therefore really only on the aspect and not the combination of the target and aspect.
