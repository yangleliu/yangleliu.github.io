---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

I am Yangle Liu, an undergraduate student at the University of Liverpool. My research spans computer vision/graphics and machine learning, with interests in LLMs, real-time scene understanding and editing, high-fidelity rendering, and data-driven methods for robust visual computing.


I am jointly supervised by [Prof. Jieming Ma](https://scholar.xjtlu.edu.cn/en/persons/JiemingMa) (Xi’an Jiaotong–Liverpool University). Additionally, I have engaged in extensive collaborative research with international scholars such as [Prof. Hai-Ning Liang](https://cma.hkust-gz.edu.cn/people/hai-ning-liang/) (HKUST–Guangzhou), [Prof. Yaochun Shen](https://www.liverpool.ac.uk/people/yaochun-shen) (University of Liverpool), and [Postdoc Bo Xiong](https://boxiong.io/) (Stanford University), all of whom remain my close academic collaborators.
# 🔥 News
- *2025.08*: &nbsp;🎉🎉 My collaborative paper will be presented as an Oral Presentation at BDAI, 2025! 
- *2024.11*: &nbsp;🎉🎉 The first collaborative paper I worked on was accepted by ICSTIS, 2024!

# 📝 Publications 
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">arXiv preprint</div><img src='/images/fruit.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[CountingFruit: Real-Time 3D Fruit Counting with Language-Guided Semantic Gaussian Splatting](https://arxiv.org/abs/2506.01109)


Fengze Li, **Yangle Liu**, Jieming Ma*, Hai-Ning Liang, Yaochun Shen, Huangxiang Li, Zhijing Wu 

[**Project**](https://fruitlanggs.github.io/) <strong><span class='show_paper_citations' data='DhtAFkwAAAAJ:ALROH1vI_8AC'></span></strong>
- We propose FruitLangGS, a language-guided 3D fruit counting framework that uses adaptive Gaussian splatting, semantic embedding, and prompt-based filtering to efficiently count fruit instances in orchard environments, even under heavy occlusion.
</div>
</div>



<div class='paper-box'><div class='paper-box-image'><div><div class="badge">BDAI 2025</div><img src='/images/seed.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[SEED: A Structural Encoder for Embedding-Driven Decoding in Time Series Prediction with LLMs](https://arxiv.org/abs/2506.20167)

<span style="color:red">(Oral Presentation)</span>

Fengze Li, Yue Wang, **Yangle Liu**, Dou Hong, Jieming Ma*, Huangxiang Li 


- We propose SEED, a structural encoder for embedding-driven decoding, designed to bridge the gap between structural representation learning and semantic inference in multivariate time series forecasting, enabling effective integration with pretrained language models for improved prediction accuracy.
</div>
</div>




<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACM TMCCA 2024</div><img src='/images/EAST.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

EAST: Environment-Aware Stylized Transition Along the Reality-Virtuality Continuum

*Under Review*

Xiaohan Zhang, Kan Liu, **Yangle Liu**, Fangze Li, Jieming Ma and Yue Li* 


- We propose EAST (Environment-Aware Stylized Transition), a framework that uses 3D Gaussian Splatting and style transfer techniques to seamlessly integrate real-world interruptions into virtual environments, ensuring aesthetic consistency and minimizing disruption along the reality-virtuality continuum.
</div>
</div>





<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICSTIS 2024</div><img src='/images/car.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Automated Generation of Parking Data Sets for Underground Car Parks](https://doi.org/10.4271/2025-01-7191)


Jiakai Li, **Yangle Liu**, Zheng Rong


- We propose a method using Blender software to generate synthetic underground parking datasets for autonomous driving, addressing challenges in data acquisition and annotation, and providing open-source resources for further development. 
</div>
</div>



# 🎖 Honors and Awards

- *2023* RoboMaster Super Competition: First Prize (Regional), Second Prize (National) 
- *2023* College Student Information System Innovation Competition: Outstanding Award
- *2023* Campus Technology Innovation Association: Managed 3D Modeling Project
- *2022* Campus Ambassador for XJTLU: Achieved promotional targets with six schools, received Pioneer Award 

# 📖 Educations
- *2024.09 - now*, Undergraduate, University of Liverpool, UK.
- *2022.09 - 2024.06*, Undergraduate, Xi’an Jiaotong–Liverpool University, Suzhou.



# 💻 Internships
<div class='paper-box'><div class='paper-box-image'><div><img src='/images/Neurova.jpg' alt="sym" style="width:150px; height:100px; object-fit:cover;"></div></div>
<div class='paper-box-text' markdown="1">

Neurova, New York

Machine Learning Intern 

*2025.06 - 2025.08*

</div>
</div>



<div class='paper-box'><div class='paper-box-image'><div><img src='/images/auo (2).png' alt="sym" style="width:100px; height:100px; object-fit:cover;"></div></div>
<div class='paper-box-text' markdown="1">

AUO, Suzhou

Software Development Intern, NUVA Platform Development Department 

*2024.06 - 2024.08*

</div>
</div>


<!-- 文末插入：地球容器 -->
<div id="globeViz" style="width:340px;height:340px;margin:32px auto;"></div>

<script src="https://unpkg.com/globe.gl"></script>
<script>
  // 若主题渲染后还有内容追加，这段会把地球容器再次移到页末，确保“文末显示”
  document.addEventListener('DOMContentLoaded', () => {
    const content = document.querySelector('.page__content') || document.querySelector('main');
    const el = document.getElementById('globeViz');
    if (content && el && el.parentNode !== content) content.appendChild(el);
  });

  const globe = Globe()
    .backgroundColor('#ffffff')                                   // 白色背景
    .globeImageUrl('//unpkg.com/three-globe/example/img/earth-day.jpg')
    .width(340).height(340);

  // 你的城市坐标
  const cities = [
    { lat: 31.3017, lng: 120.5811, name: 'Suzhou' },
    { lat: 31.00,   lng: 121.25,   name: 'Shanghai' },
    { lat: 23.128994, lng: 113.253250, name: 'Guangzhou' },
    { lat: 37.7749,   lng: -122.4194,  name: 'San Francisco' },
    { lat: 53.4084,   lng: -2.9916,    name: 'Liverpool' },
    { lat: 51.5074,   lng: -0.1278,    name: 'London' },
    { lat: 52.2053,   lng:  0.1218,    name: 'Cambridge' },
    { lat: 48.7758,   lng:  9.1829,    name: 'Stuttgart' }
  ];

  globe(document.getElementById('globeViz'))
    .pointsData(cities)
    .pointColor(() => 'red')        // 标记改为红色
    .pointRadius(0.55)
    .pointLabel(d => d.name);

  // 自动旋转
  globe.controls().autoRotate = true;
  globe.controls().autoRotateSpeed = 0.6;
</script>


