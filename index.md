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

# Find us
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d990.9161790323222!2d-7.086830533000728!3d52.24679505819285!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0xa72ff504c91913a!2sBank+Of+Ireland!5e0!3m2!1sen!2sie!4v1495180489996" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>

<!-- FB integration-->
<div id="fb-root"></div>
<script>(function(d, s, id) {
  var js, fjs = d.getElementsByTagName(s)[0];
  if (d.getElementById(id)) return;
  js = d.createElement(s); js.id = id;
  js.src = "//connect.facebook.net/en_GB/sdk.js#xfbml=1&version=v2.10&appId=403070956557717";
  fjs.parentNode.insertBefore(js, fjs);
}(document, 'script', 'facebook-jssdk'));</script>

# Social media

<div class="fb-follow" data-href="https://www.facebook.com/coderdojoardkeen/" data-layout="standard" data-size="small" data-show-faces="true"></div>

<hr>
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/">
<img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/80x15.png" /></a> Coder Dojo Ardkeen website is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons License</a>.

<!-- Chat integration-->
<script>
  ((window.gitter = {}).chat = {}).options = {
    room: 'Coderdojo-Ardkeen/Lobby'
  };
</script>
<script src="https://sidecar.gitter.im/dist/sidecar.v1.js" async defer></script>