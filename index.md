### Hi there! 👋

I'm Daniel, a CS student at Columbia University SEAS '23.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/daniel-greco-8345b3133)


- 🔭 I'm an incoming SDE at Amazon SCOT.
- 🌱 I’m currently working on setting up a web scraping library for my Open Source Development course. &rarr; [![easierscrape](https://img.shields.io/badge/repo-easierscrape-blue)](https://github.com/dag2226/easierscrape)
- ✨ I am interested in back-end and full stack development.
 
 ## Projects

{% assign orderedRepos = site.github.public_repositories | sort: 'stargazers_count' | reverse %}
{% for repository in orderedRepos %}
{% assign homepageLength = repository.homepage | size %}
{% if homepageLength > 0 %}
### {{repository.name}} | [repo]({{ repository.html_url }}) | [pages]({{ repository.homepage }}) 
{% else %}
### {{repository.name}} | [repo]({{ repository.html_url }})
{% endif %}
<div style="border-left: 3px solid #CCC; padding-left: 10px; margin-bottom: 30px">
<i>{{repository.description}}</i>
<p style="margin-top: 5px"><span style="margin-right:10px">{% octicon repo-forked size:small%} {{repository.forks_count}}</span> {% octicon star size:small %} {{repository.stargazers_count}} </p>
</div>

{% endfor %}

[![GitHub Streak](https://streak-stats.demolab.com/?user=dag2226)](https://git.io/streak-stats)
