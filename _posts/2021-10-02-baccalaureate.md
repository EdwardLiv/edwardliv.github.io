---
layout: post
title: "Baccalaureate Data Visualization"
subtitle: "How did Romanian highschoolers perform at the national exam?"
background: '/img/posts/baccalaureate/books.jpg'
---

## Past results

<iframe src="/img/posts/baccalaureate/fig_scatter_1.html" height="500px" width="100%" frameBorder="0" scrolling="no"></iframe>

## The urban-rural divide

Urban highschool students are far more likely to pass the exam (71%) than their rural counterparts (56%). Nevertheless, this isn’t the only worrying statistic.
According to the [National Institute of Statistics](https://insse.ro/cms/files/publicatii/Romania_in_cifre_breviar_statistic_2018.pdf), 46% of Romania’s population lived in rural areas in 2017. However, students that go to rural highschools account for only 32% of all Baccalaureate participants. This can be a sign of rural families that prefer urban highschools or a sign of high dropout rates in rural areas.

<iframe src="/img/posts/baccalaureate/fig_bar_1.html" height="350px" width="100%" frameBorder="0" scrolling="no"></iframe>

## Girls perform better than boys

Girls are more likely to pass the Baccalaureate (71%) than boys are (60%). The latter are prone to getting eliminated for trying to cheat the exam (115 compared to 32 girls eliminated) despite there being fewer boys participating in the national exam. This can be explained by their risk-taking behavior, or maybe girls are better at not getting caught by the teachers. Boys are also more likely to not show up at the exam (6%) than girls (4%).

<iframe src="/img/posts/baccalaureate/fig_bar_2.html" height="350px" width="100%" frameBorder="0" scrolling="no"></iframe>

## School specialization matters

Romanian highschools have a wide variety of specializations to choose from. We can view them on the following treemap chart, which is composed of rectangles ordered from largest to smallest. The area of each rectangle is determined by the number of students. The most popular specialization is “Matematică-Informatică” (24275 students).

<iframe src="/img/posts/baccalaureate/fig_treemap_1.html" height="600px" width="100%" frameBorder="0" scrolling="no"></iframe>

Although it is known that students from certain specializations perform better, there are few official sources or mainstream news that show this gap statistically. Coloring the treemap proportionally with the pass rate, we can observe huge differences. For example, 85% of “Matematică-Informatică” students passed, whereas only 10% of “Tehnician în agricultură” students passed.

<iframe src="/img/posts/baccalaureate/fig_treemap_2.html" height="600px" width="100%" frameBorder="0" scrolling="no"></iframe>

Students can pick the subject of their third test. The most popular choice is anatomy (72% pass rate). Almost all students that picked chemistry and physics have passed (96% and 94%).

<iframe src="/img/posts/baccalaureate/fig_treemap_3.html" height="600px" width="100%" frameBorder="0" scrolling="no"></iframe>

## Biased grading

In order to pass the exam, the student needs a grade higher than 5 in each test and an average of 6. Out of 127.001 non-absent candidates, 146 managed to get a perfect grade average.

<iframe src="/img/posts/baccalaureate/fig_histogram_1.html" height="500px" width="100%" frameBorder="0" scrolling="no"></iframe>

Rather than look at the final grade histogram, it’s more interesting to break it down into the multiple exams to observe some patterns. There are three big numerical spikes:
- grade 1.00: students that didn’t prepare at all for the exam
- grade 5.00: students that barely passed
- grade 10.00: students with maximum grade

Notice the big dropoff just below the pass grade threshold followed by a huge spike. There are barely any students in the 4.90-4.99 range, while the next one has a hundred times more students. Some teachers would rather artificially increase the grade to 5 than to fail a 4.9 student.

<iframe src="/img/posts/baccalaureate/fig_histogram_2.html" height="500px" width="100%" frameBorder="0" scrolling="no"></iframe>

The second exam (mathemathics or history) has the highest number of students that couldn't even get 0.1 points (2822 students).

<iframe src="/img/posts/baccalaureate/fig_histogram_3.html" height="500px" width="100%" frameBorder="0" scrolling="no"></iframe>

The third exam, which has a selectable subject, is the easiest one to get a high grade: 7223 students managed to obtain the maximum grade, compared to 2723 and 1354 at the other exams.

<iframe src="/img/posts/baccalaureate/fig_histogram_4.html" height="500px" width="100%" frameBorder="0" scrolling="no"></iframe>