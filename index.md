---
layout: default
title: Home
---

Welcome to CoderDojo Ardkeen Waterford

CoderDojo is a movement orientated around running free not-for-profit coding clubs and regular sessions for young people. At a CoderDojo, young people learn how to code, develop websites, apps, programs, games and more. Dojos are set up, run by and taught at by volunteers. In addition to learning to code, members meet like minded people, show off what they’ve been working on and so on. CoderDojo makes development and learning to code a fun, sociable, kick ass experience. CoderDojo also puts a strong emphasis on open source and free software, and has a strong network of members and volunteers globally.

![foto](/assets/session1.jpg)


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

 - Age Group 7yrs to 16 yrs.
 - A laptop. Borrow one from someone if needs be.
 - Coder Dojo ticket - due to limited spaces each coder needs to have ticket for session.
 - A parent! (Very important). If you are 11 or under, your parent must stay with you during the session.

#  What we do

See [projects](/project) page for more details.

## Find us
<iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d305.3504486251061!2d-7.0843315!3d52.2469511!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4842c6aaf30fb297%3A0x342934dc18b4aef1!2sAIB+Bank!5e0!3m2!1sen!2sie!4v1495143924004" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
