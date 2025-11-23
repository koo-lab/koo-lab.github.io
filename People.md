---
title: People
permalink: /People/
---

{% assign people_sorted = site.people | sort: 'joined' %}
{% assign people_sorted = (site.people | sort: 'joined' %}
{% assign people_array = "pi|staff|postdoc|gradstudent|postbac|undergrad|highschool" | split: "|" %}

{% for item in people_array %}

<div class="pos_header">
{% if item == 'pi' %}
<h3>Principal Investigator</h3>
 {% elsif item == 'postdoc' %}
<h3>Postdoctoral Researchers</h3>
 {% elsif item == 'gradstudent' %}
<h3>Graduate Students</h3>
 {% elsif item == 'rotation' %}
<h3>Masters Researchers</h3>
 {% elsif item == 'postbac' %}
<h3>Postbaccalaureate Researchers</h3>
 {% elsif item == 'highschool' %}
<h3>High School Researchers</h3>
{% endif %}
</div>

<div class="content list people">
  {% for profile in people_sorted %}
    {% if profile.position contains item %}
    <div class="list-item-people">
      <p class="list-post-title">
        <a href="{{ site.baseurl }}{{ profile.url }}"><img width="200" src="{{site.baseurl}}/images/people/{{profile.avatar}}"></a>
        <a class="name" href="{{ site.baseurl }}{{ profile.url }}">{{ profile.name }}</a>
      </p>
    </div>    
    {% endif %}
  {% endfor %}
</div>
<hr>
{% endfor %}


<h3>Alumni</h3>

<h5>Postdocs</h5>

| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Evan Seitz | Postdoc | CSHL | 2022-2025 | ML Research Scientist at InstaDeep |
Jessica Zhou | Postdoc | CSHL | 2023-2025 | Data Scientist at Stripe |
Yinan Dong | Postdoc | CSHL | 2023-2023 | ML Research Scientist at Meta |
Antonio Majdandzic | Postdoc | CSHL | 2020-2022 | ML Researcher at Bloomberg |
Rohit Tripathy | Postdoc | CSHL | 2020-2022 | Staff Scientist at Jackson Laboratory |

<h5>Grad Students</h5>

| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Chandana Rajesh | Grad Student | SBU Applied Math and Statistics | 2021-2025 | ML Research Scientist at InstaDeep |
Jakub Kaczmarzyk | Grad Student | SBU MD/PhD | 2021-2025 | Finishing up Med School |
Shushan Toneyan | Grad Student | CSHL | 2020-2024 | ML Research Scientist at Genentech |
Ziqi (Amber) Tang | Grad Student | CSHL | 2020-2024 | ML Research Scientist at InstaDeep |


<h5>Staff</h5>

| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Nicholas Lee | Comp Sci Developer | CSHL | 2020-2022 | |


<h5>Postbac</h5>

| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Nirali Somia | Researcher | PREP Scholar | 2024-2025 | PhD student at MIT|


<h5>Undergrads</h5>

| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Tianhao Luo | Summer Undergrad Research Program | UPenn, Statistics | Summer 2023 | PhD student at Harvard |
Nika Chuzhoy | Undergrad Researcher | CalTech, Computer Science | Summer 2023 | |
Phillip Zhou | Summer Undergrad Research Program  | Amherst College, Math | Summer 2022 | |
Vandana Agarwala | Summer Undergrad Research Program | Penn State, Computer Science | Summer 2021 | Software developer at Flagship Pioneering |
Roshan Kenia | Undergrad Researcher | Stony Brook, Computer Science | 2020-2021 | PhD student at Harvard |


<h5>High Schoolers</h5>
 
| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Arnav Pemmaraju |  High School Researcher | Great Neck South High | Summer 2025 |  |
Brian Cheng |  High School Researcher | Great Neck South High | Summer 2025 |  |
Eliot Bih |  High School Researcher | Syosset High | Summer 2025 |  |
Shivani Muthukumar | High School Researcher  | Commack High | 2024-2025 | Undergrad at Columbia |
Aayush Prakash | High School Researcher  | Half Hallow Hills High | 2022-2024 | Undergrad at UNC |
Katie Engel | High School Researcher  | Cold Spring Harbor High | 2023-2024 | Undergrad at Tufts |
Steven Yu | High School Researcher  | Syosset High | 2022-2023 | Undergrad at Columbia |
Amanda Nemshin | High School Researcher  | Cold Spring Harbor High | 2022-2023 | Undergrad at Duke |
Rohan Ghotra | High School Researcher  | Syosset High | 2021-2022 | Undergrad at Columbia |
Ethan Labelson | High School Researcher  | Friends Academy | 2021-2022 | Undergrad at Caltech |
Ashwin Narayanan | High School Researcher  | Jericho High | Summer 2022 | Undergrad at Johns Hopkins |
Zaara Yakub | High School Researcher | Bethpage High School | 2020-2021 | Undergrad at Lehigh |

<h5>Visiting researchers</h5>

| Name | Position | Program | Time in Lab | Current Position |
| :------------- |:-------------| :-----------| :-----------| :-----------|
Eduardo Esteva | Masters Student | NYU, Bioinformatics | 2020-2021 | Bioinformatics Analyst at NYU Grossman School of Medicine |


<br>
<br>
<br>


