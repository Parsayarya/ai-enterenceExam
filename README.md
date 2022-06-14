# ai-enterenceExam
First I sorted the file based on the speakers,highlighted the outliers then started to notice that some of the rows of speaker/voices don't have sufficient data.
Then based on that observation I reached to the conclusion that diffrent voices/categories can not be judged by the same criteria.
After that I moved on to calculating the error percentages.
/n
**first question**
There are several basic issues with the distribution of the errors for example the fact that we have no (خطای اعراب) errors wich could be the result of classifying those errors as other ones for example(خطای نگارش) or (خطای پیاده سازی) other than that the fact that we had the same amount of (خطای اعداد )  errors as (خطای کمتر از 10) errors seemed a bit strange.
Then there was the issue of (کلمات دخیل ) error which was a lot more than the expected amount which could have some implications with the method which was implemented to catch this kind of error how catching.
generally speaking because we had a lot more data from category(الف) the errors were more clear and there was finer understanding of what the data actually lacked.
Almost the same could be articulated for (ب)  category but the (ج)  category was inable to clerify a lot of errors.
**second question**
First of all for (کلمات دخیل ) error there should be a standardized immutable table of certain tokens in order to lower the misunderstanding between editors and machine on what token,word actually indicates an (کلمات دخیل ) error.
Then there is the issue of (ج)  category, there isn't sufficient data so eighter adding to it or generating data based on what we have using Data Augmentation because whta we have now shows signs of over-fitting.
There is definitely a problem with (خطای اعراب) errors they are eighter being classified as other errors leading to more erors in areas that we didn't expect and making us believe that our data or model or editors are lacking so we should certainly revisit the criteria we set for cathing the said error.
**third question**
Some errors such as (خطای نگارش) , (خطای اعراب) , (خطای اعداد )  have the same source,if the model edited itself properly almost none of them would be remaining.
other errors like (خطای کمتر از 10),(خطای بیشتر از 50) and  (خطای پیاده سازی) come from the NLP model  or our speakers and the (کلمات دخیل ) error i would say is unquestionably related to editors.
