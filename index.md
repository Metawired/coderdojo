---
layout: default
title: Home
---

<div class="jumbotron">
  <h1 class="display-3">Welcome to CoderDojo Ardkeen Waterford!</h1>
  <p class="lead">
    CoderDojo is a movement orientated around running free not-for-profit coding clubs and regular sessions for young people. At a CoderDojo, young people learn how to code, develop websites, apps, programs, games and more. CoderDojo also puts a strong emphasis on open source and free software, and has a strong network of members and volunteers globally.
  </p>
  <hr class="my-4">
  <p>

  </p>
  <p class="lead">
    <a class="btn btn-primary btn-lg" href="{{site.url}}/project" role="button">Learn more</a>
  </p>
</div>

# Upcoming events

{% for event in site.data.events %}
## {{event.name}}
{% if event.date != nil %}
{{ event.date | date_to_string }} at {{ event.time }}
{% endif %}
{% if event.detail != nil %}
{{ event.detail | markdownify }}
{% endif %}
{% endfor %}

#  What's required to join us:

 - Age from 9 to 16 years.
 - A laptop. Borrow one from someone if needs be.
 - Coder Dojo ticket - due to limited spaces each coder needs to reserve seat for session.
 - A parent! (Very important). If you are 11 or under, your parent must stay with you during the session.

#  Want to join us?

See [Getting started](/project/starter) page for more details.

#  What we do

See [projects](/project) page for more details.