---
permalink: /
title: "Welcome"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Welcome to my website. I am a <u>Computer Science Ph.D.</u> student at <u>Arizona State University</u> and a research assistant at <u>ASU-Mayo Center for Innovative Imaging</u> ([AMCII](https://amcii.asu.edu/)). My advisor is <u>Professor Baoxin Li</u>, and my co-advisor is <u>Professor Teresa Wu</u>. My research interests lie in developing computer vision methods for medical image analysis—including but not limited to the tasks of supervised, weakly-supervised, self-supervised, and unsupervised lesion segmentation, detection, and classification. I serve as a reviewer in many conferences and journals in my field. I have received <u>IEEE TMI Distinguished Reviewer—Bronze Level</u> and <u>IEEE TMI Distinguished Reviewer—Silver Level</u> awards from <u>IEEE Transactions on Medical Imaging</u> and <u>Certificate of Outstanding Contribution in Reviewing</u> from the <u>Journal of Biomedical Informatics</u>. I also worked as <u>Applied Research Intern (Medical Imaging)</u> at <u>NVIDIA</u> during the summer of 2021 and 2022.

My complete CV is available [here](/cv). You can also download my CV in pdf format from [here](/files/CV_md_mahfuzur.pdf).

Recent News
======
- Sep 14, 2022: Paper accepted at **Brain Communications**.
- Aug 27, 2022: I have received **IEEE TMI Distinguished Reviewer—Silver Level** from IEEE Transactions on Medical Imaging.

Recent Blog Posts
======

<ul>
{% for post in site.posts %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% if year != written_year %}
    {% capture written_year %}{{ year }}{% endcapture %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}
</ul>
