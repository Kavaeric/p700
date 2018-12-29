---
layout: default
title: Sol
accent: var(--cl-yellow)
section: Codex
categories: Locations
---

{% include infobox_star.html 
    name="Sol"
    quarter="Terran Core Quarter"
    catname="Sol a"
    cattime="Ancient"
    demonym="Solar"

    class="G2V"
    mag="4.83"
    temp="5,773"

    mass="1.99 &#215; 10<sup>30</sup>"
    relmass="1" 
    radius="696,400" 
    relradius="1"
    grav="274"
    age="4.45 Gy"
    
    pop="~15.6 billion"
    affil="[Terran Federation](Terran_Federation)"
    settled="Prehistoric"
%}

**Sol** is a main-sequence yellow star of spectral class G2V, and is the most populated star system
in all of [Juxta Sagittaria](Juxta_Sagittaria). Sol is believed to be approximately 4.5 billion
years old.

Sol is orbited by [Earth](Earth), the capital and homeworld of the [Terran Federation](Terran_Federation).
Terrans have a consistent presence throughout the Sol system due to the abundance of lucrative mining
sites across Sol's various planets, moons, and asteroids.

## Solar system
The Solar system has eight planets: Four inner terrestrial planets, two gas giants, and two ice giants.

<div class="systemDiagram">
    {% include system_object.html 
        name="Sol"
        type="star"
        diameter="5"
    %}
    {% include system_object.html 
        name="Mercury"
        article="Mercury"
        type="body"
        diameter="1"
    %}
    {% include system_object.html 
        name="Venus"
        article="Venus"
        type="body"
        diameter="1.3"
    %}
    {% capture luna %}{% include system_moon.html name='Luna' article='Luna.html' diameter='.75' %}{% endcapture %}
    {% include system_object.html 
        name="Earth"
        article="Earth"
        type="body"
        diameter="1.5"
        moons=luna
    %}
    {% capture marsmoons %}
    {% include system_moon.html name='Phobos' diameter='.5' %}
    {% include system_moon.html name='Deimos' diameter='.5' %}
    {% endcapture %}
    {% include system_object.html 
        name="Mars"
        article="Mars"
        type="body"
        diameter="1.1"
        moons=marsmoons
    %}

    {% capture asteroids %}
    {% include system_moon.html name='Ceres' diameter='.5' %}
    {% endcapture %}
    {% include system_object.html
        name="Asteroid belt"
        article="Solar_asteroid_belt.html"
        type="belt"
        moons=asteroids
    %}

    {% capture jupitermoons %}
    {% include system_moon.html name='Io' diameter='.8' %}
    {% include system_moon.html name='Europa' diameter='.65' %}
    {% include system_moon.html name='Ganymede' diameter='.75' %}
    {% include system_moon.html name='Callisto' diameter='.8' %}
    {% endcapture %}
    {% include system_object.html 
        name="Jupiter"
        article="Jupiter"
        type="body"
        diameter="3.5"
        moons=jupitermoons
    %}
    {% capture saturnmoons %}
    {% include system_moon.html name='Titan' diameter='.75' %}
    {% endcapture %}
    {% include system_object.html 
        name="Saturn"
        article="Saturn"
        type="body"
        diameter="3"
        axis="27"
        moons=saturnmoons
        ringsize="1.8"
    %}
    {% capture uranusmoons %}
    {% include system_moon.html name='Miranda' diameter='.3' %}
    {% include system_moon.html name='Ariel' diameter='.5' %}
    {% include system_moon.html name='Umbra' diameter='.5' %}
    {% include system_moon.html name='Titania' diameter='.5' %}
    {% include system_moon.html name='Oberon' diameter='.5' %}
    {% endcapture %}
    {% include system_object.html 
        name="Uranus"
        article="Uranus"
        type="body"
        diameter="2.5"
        axis="98"
        moons=uranusmoons
        ringsize="1"
    %}
    {% capture neptunemoons %}
    {% include system_moon.html name='Triton' diameter='.5' %}
    {% endcapture %}
    {% include system_object.html 
        name="Neptune"
        article="Neptune"
        type="body"
        diameter="2.4"
        moons=neptunemoons
    %}
</div>
