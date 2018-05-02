### My Repositories

##### Hobby Projects and Contributions:
{% for repository in site.github.public_repositories %}
 {% if repository.archived  or repository.name == 'sagarchalise.github.io' %}
{% else %}
  * [{{ repository.name }}]({{ repository.html_url }}){% if repository.language %} [Language: {{repository.language}}]{% endif %}
    >{{repository.description or repository.homepage}}
 {% endif %}
{% endfor %}

###### Archived Projects
{% for repository in site.github.public_repositories %}
{% if repository.archived %}
+ {{ repository.name }}{% if repository.language %} [Language: {{repository.language}}]{% endif %}
{% endif %}
{% endfor %}
