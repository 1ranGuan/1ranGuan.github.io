<h2 id="publications">Publications</h2>

(*Equal contribution, †Corresponding authors)

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3">
    {% if link.image %}
    <img src="{{ link.image }}" class="teaser" alt="{{ link.title }}">
    {% endif %}
  </div>
  <div class="col-sm-9">
    <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
    <div class="author">{{ link.authors }}</div>
    <div class="periodical"><em>{{ link.conference }}</em></div>
    <div class="links">
      {% if link.pdf %}
      <a href="{{ link.pdf }}" target="_blank">PDF</a>
      {% endif %}
      {% if link.code %}
      <a href="{{ link.code }}" target="_blank">Code</a>
      {% endif %}
      {% if link.page %}
      <a href="{{ link.page }}" target="_blank">Project</a>
      {% endif %}
      {% if link.bibtex %}
      <a href="{{ link.bibtex }}" target="_blank">BibTeX</a>
      {% endif %}
      {% if link.notes %}
      <strong class="pub-note">{{ link.notes }}</strong>
      {% endif %}
    </div>
  </div>
</div>
</li>

{% endfor %}

</ol>
</div>
