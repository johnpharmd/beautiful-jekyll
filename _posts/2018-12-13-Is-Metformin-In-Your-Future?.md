---
title: Is Metformin In Your Future?
subtitle: And why maybe it should be
---

America’s not perfect. No newsflash, that. But one problem in particular is looming massive by 2050. **One third of *all* of the U.S. will have developed diabetes by then**, if current [trends hold]( https://www.einstein.yu.edu/centers/diabetes-research/facts-statistics/).

Yes, you read that right. One-third of Americans. Huge problem, no? What can we do?

Well, some scientists are recommending that many folks without diabetes take a unique, well-studied medicine called [metformin]( https://www.wired.com/story/this-pill-promises-to-extend-life-for-a-nickel-a-pop/). But metformin is usually started only *after* a physician’s diagnosis of type 2 diabetes mellitus. That’s the current [FDA indication](https://www.fda.gov/Drugs/DrugSafety/PostmarketDrugSafetyInformationforPatientsandProviders/ucm493293.htm). I looked at [this UC Irvine Dataset](https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008#) to try to get a sense of whether *prophylactic* metformin might lessen human suffering.

Here’s a snapshot of what I did; see my Google [Colab notebook](https://colab.research.google.com/drive/12Bq7-w3PnGDxhIH7UDmj5NXQZi_Y41uv) for full details. In addition to using the forementioned data, I mapped [ICD-9 data](https://github.com/drobbins/ICD9) from David Robbins--thanks, David!--to the data, but without joining datasets. Am proud of columns 5 through 9. I observed these top values for the wrangled main dataset. Hat tip to Python3 and pandas!

![img-1](/img/2018-12-13-blog-img1.png)

Now, before you clamor about non-generalizability, please consider that really only "race" is highly skewed here. (I prefer "ethnicity", but that's a topic for another post.)

Given my work as a clinical pharmacist (including in more than one hospital), it didn't surprise me that number of diagnoses increased with age, but I wanted to visualize it a la seaborn.

![img-2](/img/2018-12-13-blog-img2.png)

Here, I show age brackets versus the metformin class label.

![img-3](/img/2018-12-13-blog-img3.PNG)

So this mini-analysis wouldn't be complete without at least one statistical test, right? I ran a t-test for independent samples on the crosstab of number of diagnoses versus the potential class label of taking/not taking metformin.



(Give my conclusion.)
