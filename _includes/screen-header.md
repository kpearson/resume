{% if site.resume_avatar == 'true' %}
<img src="images/avatar.png" alt="my photo" class="avatar" itemprop="image">
{% endif %}

<h1 class="header-name" itemprop="name">{{ site.resume_name }}</h1>

<div class="title-bar">

  <h2 class="header-title" itemprop="jobTitle">{{ site.resume_title }}</h2>

  {% include icon-links.html %}
</div>

<div class="executive-summary" itemprop="description">
  <p>{% include summery.md %}</p>
</div>

{% if site.resume_looking_for_work == 'yes' %}
<a href="mailto:{{ site.resume_contact_email }}" class="contact-button" itemprop="email">Contact me</a>
{% elsif site.resume_looking_for_work == 'no' %}
<a class="contact-button not-looking">I'm not looking for work right now.</a>
{% else %}
{% endif %}
