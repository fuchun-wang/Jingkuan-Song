---
layout: page
permalink: /
title: about
nav: about

<!--description: <a href="https://ai.google/" target="_blank">Google AI</a> -->
address: <a href="https://www.google.com/maps/place/Googleplex/@37.4220656,-122.0862837,17z/data=!3m1!4b1!4m5!3m4!1s0x808fba02425dad8f:0x6c296c66619367e0!8m2!3d37.4220656!4d-122.0840897" class="page-description" target="_blank">Googleplex, Mountain View, California, USA </a>
---

<div class="col p-0 pt-4 pb-4">
  <h1 class="pb-3 title text-left font-weight-bold">Jingkuan Song</h1>
  <h6 class="m-0 mb-2" style="font-size: 0.83em;">{{ page.description }}</h6>
  {% if page.address %}
      <h6 class="m-0 mb-2" style="font-size: 0.83em;">{{ page.address }}</h6>
  {% endif %}
</div>

<!-- Introduction -->

<div style="display: flex; flex-wrap: wrap;">
    <div class="text-justify p-0">
        <div class="col-xs-12 col-sm-6 p-0 pt-2 pb-sm-2 pb-4 pl-sm-4 text-center" style="float: right;">
          <img class="profile-img img-responsive" src="{{ 'prof_pic.jpg' | prepend: '/assets/img/' | prepend: site.baseurl | prepend: site.url }}">
        </div>

        <p>
            Jingkuan Song is a full professor with [University of Electronic Science and Technology of China (UESTC)](https://www.uestc.edu.cn/). He joined [Columbia University](https://www.columbia.edu/) as a Postdoc Research Scientist (2016-2017), and [University of Trento](http://www.unitn.it/) as a Research Fellow (2014-2016). He obtained his PhD degree in 2014 from The University of Queensland (UQ), Australia (advised by [Prof. Heng Tao Shen](https://cfm.uestc.edu.cn/~shenht/)). His research interest includes large-scale multimedia retrieval, image/video segmentation and image/video understading using hashing, graph learning and deep learning techniques. He was the winner of the Best Paper Award in ICPR (2016, Mexico), Best Student Paper Award in Australian Database Conference (2017, Australia), and Best Paper Honorable Mention Award (2017, Japan). He is Guest Editor of TMM, WWWJ and he is PC member of CVPR’18, MM'18, IJCAI'18, etc.
        </p>
        
        <p>
            I am looking for highly motivated PhD students, Postdoctorals and Assistant Professors to conduct world-class research in my team. Please send your CV or enquiries to my email.
        </p>
    </div>
</div>

<div class="col text-justify p-0">
    <p>
        Before I joined CMU, I graduated with an <a href="https://www.cst.cam.ac.uk/admissions/acs" target="_blank">M.Phil. in Advanced Computer Science</a>
        from the <a href="https://www.cam.ac.uk/" target="_blank">University of Cambridge</a>, UK.
        In my Master's thesis I used Machine Learning methods to detect and align chromosomes in microscope images,
        advised by <a href="https://www.cl.cam.ac.uk/~pl219/" target="_blank">Pietro Lió</a>.
    </p>
</div>

<!-- News -->
<div class="news mt-3 p-0">
  <h1 class="title mb-4 p-0">news</h1>
  {% assign news = site.news | reverse %}
  {% for item in news limit: site.news_limit %}
    <div class="row p-0">
      <div class="col-sm-2 p-0">
        <span class="badge light-green darken-1 font-weight-bold text-uppercase align-middle date ml-3">
          {{ item.date | date: "%b %-d, %Y" }}
        </span>
      </div>
      <div class="col-sm-10 mt-2 mt-sm-0 ml-3 ml-md-0 p-0 font-weight-light text">
        <p>{{ item.content | remove: '<p>' | remove: '</p>' | emojify }}</p>
      </div>
    </div>
  {% endfor %}
</div>
