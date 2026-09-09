<h2 id="publications" style="margin: 2px 0px -5px;">Publications</h2>

<div class="publications">

<!-- ============================================================
     International Conferences
============================================================ -->

<h3 style="margin-top: 25px; margin-bottom: 15px;">
  International Conferences
</h3>

<ol class="bibliography">

{% for link in site.data.publications.conferences %}

<li>
<div class="pub-row">

  <!-- Image -->
  <div class="col-sm-3 abbr"
       style="position: relative; padding-right: 15px; padding-left: 15px;">

    {% if link.image %}
    <img src="{{ link.image }}"
         class="teaser img-fluid z-depth-1"
         style="width=100;height=40%">

      {% if link.conference_short %}
      <abbr class="badge">{{ link.conference_short }}</abbr>
      {% endif %}

    {% endif %}

  </div>


  <!-- Publication Information -->
  <div class="col-sm-9"
       style="position: relative; padding-right: 15px; padding-left: 20px;">

    <div class="title">
      {% if link.pdf %}
      <a href="{{ link.pdf }}" target="_blank">
        {{ link.title }}
      </a>
      {% else %}
        {{ link.title }}
      {% endif %}
    </div>

    <div class="author">
      {{ link.authors }}
    </div>

    <div class="periodical">
      <em>{{ link.conference }}</em>
    </div>


    <div class="links">

      <!-- PDF -->
      {% if link.pdf %}
      <a href="{{ link.pdf }}"
         class="btn btn-sm z-depth-0"
         role="button"
         target="_blank"
         style="font-size:12px;">
        PDF
      </a>
      {% endif %}


      <!-- Code -->
      {% if link.code %}
      <a href="{{ link.code }}"
         class="btn btn-sm z-depth-0"
         role="button"
         target="_blank"
         style="font-size:12px;">
        Code
      </a>
      {% endif %}


      <!-- BibTeX -->
      {% if link.bibtex %}
      <a href="{{ link.bibtex }}"
         class="btn btn-sm z-depth-0"
         role="button"
         target="_blank"
         style="font-size:12px;">
        BibTeX
      </a>
      {% endif %}


      <!-- Presentation Type -->
      {% if link.notes %}
      <strong>
        <i style="color:#e74d3c;">
          {{ link.notes }}
        </i>
      </strong>
      {% endif %}


      <!-- Award -->
      {% if link.award %}
      <span style="
        color:#d4af37;
        font-weight:700;
        margin-left:8px;
        white-space:nowrap;
      ">
        <span style="font-size:15px;">★</span>
        {{ link.award }}
      </span>
      {% endif %}

    </div>

  </div>

</div>
</li>

<br>

{% endfor %}

</ol>


<!-- ============================================================
     International Journals
============================================================ -->

<h3 style="margin-top: 35px; margin-bottom: 15px;">
  International Journals
</h3>

<ol class="bibliography">

{% for link in site.data.publications.journals %}

<li>
<div class="pub-row">

  <!-- Image -->
  <div class="col-sm-3 abbr"
       style="position: relative; padding-right: 15px; padding-left: 15px;">

    {% if link.image %}
    <img src="{{ link.image }}"
         class="teaser img-fluid z-depth-1"
         style="width=100;height=40%">

      {% if link.conference_short %}
      <abbr class="badge">{{ link.conference_short }}</abbr>
      {% endif %}

    {% endif %}

  </div>


  <!-- Publication Information -->
  <div class="col-sm-9"
       style="position: relative; padding-right: 15px; padding-left: 20px;">

    <div class="title">
      {% if link.pdf %}
      <a href="{{ link.pdf }}" target="_blank">
        {{ link.title }}
      </a>
      {% else %}
        {{ link.title }}
      {% endif %}
    </div>

    <div class="author">
      {{ link.authors }}
    </div>

    <div class="periodical">
      <em>{{ link.conference }}</em>
    </div>


    <div class="links">

      <!-- PDF -->
      {% if link.pdf %}
      <a href="{{ link.pdf }}"
         class="btn btn-sm z-depth-0"
         role="button"
         target="_blank"
         style="font-size:12px;">
        PDF
      </a>
      {% endif %}


      <!-- Code -->
      {% if link.code %}
      <a href="{{ link.code }}"
         class="btn btn-sm z-depth-0"
         role="button"
         target="_blank"
         style="font-size:12px;">
        Code
      </a>
      {% endif %}


      <!-- BibTeX -->
      {% if link.bibtex %}
      <a href="{{ link.bibtex }}"
         class="btn btn-sm z-depth-0"
         role="button"
         target="_blank"
         style="font-size:12px;">
        BibTeX
      </a>
      {% endif %}


      <!-- Notes -->
      {% if link.notes %}
      <strong>
        <i style="color:#e74d3c;">
          {{ link.notes }}
        </i>
      </strong>
      {% endif %}


      <!-- Award -->
      {% if link.award %}
      <span style="
        color:#d4af37;
        font-weight:700;
        margin-left:8px;
        white-space:nowrap;
      ">
        <span style="font-size:15px;">★</span>
        {{ link.award }}
      </span>
      {% endif %}

    </div>

  </div>

</div>
</li>

<br>

{% endfor %}

</ol>

</div>
