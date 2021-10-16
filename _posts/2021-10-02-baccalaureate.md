---
layout: post
title: "Baccalaureate Data Visualization"
subtitle: "How did Romanian high schoolers perform at the national exam?"
background: '/img/posts/baccalaureate/books.jpg'
---

The Romanian Baccalaureate is the final exam that a student must pass in order to graduate high school. Despite being an important news topic each year, there is no in-depth analysis of the results in the media. Most of the time, we only see the national pass rate and a per-county map. Therefore, I decided to write an article with figures to give some insights about the subject. 

Data is provided by the [Government’s dataset website](https://data.gov.ro/). The figures are interactive, hover over them to get more information. Be aware that I will use Romanian language for figures since it would be confusing to translate terms such as *profilul uman*.

## Past results

In recent years, the national pass rate has been around <span style="color:#1F77B4">**65-70%**</span>. Out of 127.001 non-absent students at the 2021 Summer Baccalaureate, <span style="color:#1F77B4">**69%**</span> passed the exam. Note that the Ministry of Education formula of calculating the rate does not include absent students.

<iframe src="/img/posts/baccalaureate/fig_scatter_1.html" height="500px" width="100%" frameBorder="0" scrolling="no"></iframe>

## The urban-rural divide

Urban high school students are far more likely to pass the exam <span style="color:#1F77B4">**(71%)**</span> than their rural counterparts <span style="color:#1F77B4">**(56%)**</span>. Nevertheless, this isn’t the only worrying statistic.
According to the [National Institute of Statistics](https://insse.ro/cms/files/publicatii/Romania_in_cifre_breviar_statistic_2018.pdf), 46% of Romania’s population lived in rural areas in 2017. However, students that go to rural high schools account for only <span style="color:#D62728">**32%**</span> of all Baccalaureate participants. This can be a sign of rural families that prefer urban high schools or a sign of high dropout rates in rural areas.

<iframe src="/img/posts/baccalaureate/fig_bar_1.html" height="350px" width="100%" frameBorder="0" scrolling="no"></iframe>

## Girls perform better than boys

Girls are more likely to pass the Baccalaureate <span style="color:#1F77B4">**(71%)**</span> than boys are <span style="color:#1F77B4">**(60%)**</span>. The latter are prone to getting eliminated for trying to cheat the exam (<span style="color:#D62728">**115**</span> compared to <span style="color:#D62728">**32**</span> girls eliminated) despite there being fewer boys participating in the national exam. This can be explained by their risk-taking behavior, or maybe girls are better at not getting caught by the teachers. Boys are also more likely to not show up at the exam <span style="color:#D62728">**(6%)**</span> than girls <span style="color:#D62728">**(4%)**</span>.

<iframe src="/img/posts/baccalaureate/fig_bar_2.html" height="350px" width="100%" frameBorder="0" scrolling="no"></iframe>

## School specialization matters

Romanian highs chools have a wide variety of specializations to choose from. We can view them on the following treemap chart, which is composed of rectangles ordered from largest to smallest. The area of each rectangle is determined by the number of students. The most popular specialization is *Matematică-Informatică* (24.275 students).

<iframe src="/img/posts/baccalaureate/fig_treemap_1.html" height="600px" width="100%" frameBorder="0" scrolling="no"></iframe>

Although it is known that students from certain specializations perform better, there are few official sources or mainstream news that show this gap statistically. Coloring the treemap proportionally with the pass rate, we can observe huge differences. For example, <span style="color:#1F77B4">**85%**</span> of *Matematică-Informatică* students passed, whereas only <span style="color:#D62728">**10%**</span> of *Tehnician în agricultură* students passed.

<iframe src="/img/posts/baccalaureate/fig_treemap_2.html" height="600px" width="100%" frameBorder="0" scrolling="no"></iframe>

Students can pick the subject of their third test. The most popular choice is anatomy (<span style="color:#1F77B4">**72%**</span> pass rate). Almost all students that picked chemistry and physics have passed (<span style="color:#1F77B4">**96%**</span> and <span style="color:#1F77B4">**94%**</span>).

<iframe src="/img/posts/baccalaureate/fig_treemap_3.html" height="600px" width="100%" frameBorder="0" scrolling="no"></iframe>

## Biased grading

In order to pass the exam, the student needs a grade higher than 5 in each test and an average of 6. Out of 127.001 non-absent candidates, <span style="color:#1F77B4">**146**</span> managed to get a perfect grade average.

<iframe src="/img/posts/baccalaureate/fig_histogram_1.html" height="500px" width="100%" frameBorder="0" scrolling="no"></iframe>

Rather than look at the final grade histogram, it’s more interesting to break it down into the multiple exams to observe some patterns. There are three big numerical spikes:
- grade 1.00: students that didn’t prepare at all for the exam
- grade 5.00: students that barely passed
- grade 10.00: students with maximum grade

Notice the big dropoff just below the pass grade threshold followed by a huge spike. There are barely any students in the 4.90-4.99 range, while the next one has a hundred times more students. Some teachers would rather artificially increase the grade to 5 than to fail a 4.9 student.

<iframe src="/img/posts/baccalaureate/fig_histogram_2.html" height="500px" width="100%" frameBorder="0" scrolling="no"></iframe>

The second exam (mathemathics or history) has the highest number of students that couldn't even get 0.1 points (<span style="color:#D62728">**2822 students**</span>).

<iframe src="/img/posts/baccalaureate/fig_histogram_3.html" height="500px" width="100%" frameBorder="0" scrolling="no"></iframe>

The third exam, which has a selectable subject, is the easiest one to get a high grade: <span style="color:#1F77B4">**7223**</span> students managed to obtain the maximum grade, compared to <span style="color:#1F77B4">**2723**</span> and <span style="color:#1F77B4">**1354**</span> at the other exams.

<iframe src="/img/posts/baccalaureate/fig_histogram_4.html" height="500px" width="100%" frameBorder="0" scrolling="no"></iframe>

## Conclusion

I hope you found this article helpful in understanding the students' background and the results. The figures were made in Python Plotly. The source code can be found on my [GitHub account](https://github.com/EdwardLiv) and the data on the [Government's open datasets](https://data.gov.ro/) website.