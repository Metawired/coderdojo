---
layout: default
title: Home
---

<div class="jumbotron">
  <h1 class="display-3">Welcome to CoderDojo Ardkeen Waterford!</h1>
  <p class="lead">
    CoderDojo is a movement orientated around running free not-for-profit coding clubs and regular sessions for young people. At a CoderDojo, young people learn how to code, develop websites, apps, programs, games and more. CoderDojo also puts a strong emphasis on open source and free software, and has a strong network of members and volunteers globally.
  </p>
  <div class="btn-group" role="group" aria-label="Basic example">
    <a class="btn btn-primary btn-lg" href="/project/general/starter" role="button">Want To Join Us?</a>
    <a class="btn btn-primary btn-lg" href="/project" role="button">What We Do</a>
  </div>
  <hr class="my-4">
  <div class="row">
    <div class="col-xs-12 col-sm-4">
      <div class="card bg-dark mb-0">
        <div class="card-header lead font-weight-bold">Upcoming Event</div>
        <div class="card-block">
        {% for item in site.data.events %}
          <h4 class="card-title">{{ item.name }}</h4>
          <p class="card-text">{{ item.date | date_to_long_string }} {{ item.time }}</p>
          <a href="{{ item.detail }}" class="btn btn-primary">Register Now</a>
        {% endfor %}
        </div>
      </div>
    </div>
    <div class="col-xs-12 col-sm-8">
      <ul class="list-group">
        <li class="list-group-item lead font-weight-bold">What's required to join us?</li>
        <li class="list-group-item">9-16 years old</li>
        <li class="list-group-item">A laptop. Borrow one from someone if needs be</li>
        <li class="list-group-item">Coder Dojo ticket - due to limited spaces each coder needs to reserve seat for session</li>
        <li class="list-group-item">A parent! (Very important). If you are 11 or under, your parent must stay with you during the session</li>
      </ul>
    </div>
  </div>
</div>