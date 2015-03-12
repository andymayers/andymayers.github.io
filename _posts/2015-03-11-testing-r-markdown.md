---
layout: post
title: Testing R Markdown
output: md_document
---

```{r qplot, fig.width=4, fig.height=3, message=FALSE}
ss <- as.data.frame(read.csv("/Jobs/CRP/senate\_spending\_final.csv"))
summary(ss)
library(ggplot2)
qplot(vap, total, data=ss, xlab='Voting Age Population', ylab = 'Race Spending') + geom_smooth()
```