---
layout: post
title: Testing R Markdown
output: md_document
---

```{r qplot, fig.width=4, fig.height=3, message=FALSE}
library(ggplot2)
qplot(vap, total, data=ss, xlab='Voting Age Population', ylab = 'Race Spending') + geom_smooth()
```