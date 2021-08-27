---
layout: page
title: Resources
permalink: /resources/
---
<!-- blog -->

{% for item in site.data.settings.resources-items %}
<section class="section bg-light">
<div class="container">
        <div class="col-12 text-center">
            <h2 class="section-title" style="margin-bottom: 40px;">{{ item.title }}</h2>
            <p>{{ item.fdis }}</p>
        </div>

<!-- Programming_101 -->

<div class="row row-eq-height">
            <!-- {% for label in site.data.settings.{{ item.name }} %}
            <div class="col-lg-4 col-sm-6 mb-4">
                <article class="card shadow">
                    <img class="rounded card-img-top" src="{{ site.baseurl }}/assets/images/resources/{{ label.image }}"
                        alt="{{ label.title }}">
                    <div class="card-body">
                        <h4 class="card-title"><a class="text-dark"
                                href="{{ label.link }}" target="_blank">{{ label.title }}</a></h4>
                        <p class="cars-text">{{ label.discription }}
                        </p>
                        <a href="{{ label.link }}" class="btn btn-xs btn-primary" target="_blank">Read More</a>
                    </div>
                </article>
            </div>
            {% endfor %} -->
            {% if item.name == "wiki" %}         
            {% for label in site.data.settings.wiki %}
            <div class="col-lg-4 col-sm-6 mb-4">
                <article class="card shadow">
                    <img class="rounded card-img-top" src="{{ site.baseurl }}/assets/images/resources/{{ label.image }}"
                        alt="{{ label.title }}">
                    <div class="card-body">
                        <h4 class="card-title"><a class="text-dark"
                                href="{{ label.link }}" target="_blank">{{ label.title }}</a></h4>
                        <p class="cars-text">{{ label.discription }}
                        </p>
                        <a href="{{ label.link }}" class="btn btn-xs btn-primary" target="_blank">Read More</a>
                    </div>
                </article>
            </div>
            {% endfor %}  
            {% elsif item.name == "ciq" %}
            
            {% for label in site.data.settings.ciq %}
            <div class="col-lg-4 col-sm-6 mb-4">
                <article class="card shadow">
                    <img class="rounded card-img-top" src="{{ site.baseurl }}/assets/images/resources/{{ label.image }}"
                        alt="{{ label.title }}">
                    <div class="card-body">
                        <h4 class="card-title"><a class="text-dark"
                                href="{{ label.link }}" target="_blank">{{ label.title }}</a></h4>
                        <p class="cars-text">{{ label.discription }}
                        </p>
                        <a href="{{ label.link }}" class="btn btn-xs btn-primary" target="_blank">Read More</a>
                    </div>
                </article>
            </div>
            {% endfor %}
            
         
            
            {% elsif item.name == "as" %}
            
            {% for label in site.data.settings.as %}
            <div class="col-lg-4 col-sm-6 mb-4">
                <article class="card shadow">
                    <img class="rounded card-img-top" src="{{ site.baseurl }}/assets/images/resources/{{ label.image }}"
                        alt="{{ label.title }}">
                    <div class="card-body">
                        <h4 class="card-title"><a class="text-dark"
                                href="{{ label.link }}" target="_blank">{{ label.title }}</a></h4>
                        <p class="cars-text">{{ label.discription }}
                        </p>
                        <a href="{{ label.link }}" class="btn btn-xs btn-primary" target="_blank">Read More</a>
                    </div>
                </article>
            </div>
            {% endfor %}
            
           
            {% elsif item.name == "ls21" %}
            
            {% for label in site.data.settings.ls21 %}
            <div class="col-lg-4 col-sm-6 mb-4">
                <article class="card shadow">
                    <img class="rounded card-img-top" src="{{ site.baseurl }}/assets/images/resources/{{ label.image }}"
                        alt="{{ label.title }}">
                    <div class="card-body">
                        <h4 class="card-title"><a class="text-dark"
                                href="{{ label.link }}" target="_blank">{{ label.title }}</a></h4>
                        <p class="cars-text">{{ label.discription }}
                        </p>
                        <a href="{{ label.link }}" class="btn btn-xs btn-primary" target="_blank">Read More</a>
                    </div>
                </article>
            </div>
            {% endfor %}
            
            

            {% elsif item.name == "ls" %}
            
            {% for label in site.data.settings.ls %}
            <div class="col-lg-4 col-sm-6 mb-4">
                <article class="card shadow">
                    <img class="rounded card-img-top" src="{{ site.baseurl }}/assets/images/resources/{{ label.image }}"
                        alt="{{ label.title }}">
                    <div class="card-body">
                        <h4 class="card-title"><a class="text-dark"
                                href="{{ label.link }}" target="_blank">{{ label.title }}</a></h4>
                        <p class="cars-text">{{ label.discription }}
                        </p>
                        <a href="{{ label.link }}" class="btn btn-xs btn-primary" target="_blank">Read More</a>
                    </div>
                </article>
            </div>
            {% endfor %}
            
            {% endif %}


</div>
<p class="text-center">{{ item.ldis }}</p>
<div style="display: flex; align-item: center; justify-content: center;">
<a href="{{ item.btn-link }}" class="btn btn-xs btn-primary" target="_blank" style="
    padding: 15px 30px;
    font-size: 25px;
">{{ item.btn-title }}</a>
</div>
</div>
</section>

{% endfor %}


