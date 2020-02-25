---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page

---
<div align="center">





 <div class="row">
    

<div class="column" style="background-color: #F5F5F5;box-shadow:0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);">
  
<h5 style="padding: 0.2rem; color: white; background-color: #801415; border-radius: 5px"><i class="fa fa-users mr-3"></i> <b>Comité Organizador</b></h5>




{% assign chairs = site.data.comite_organizador %}
{% for chair in chairs %}
<div style="font-size: 0.9rem; padding-top: 1.5rem; padding-bottom: 1.5rem;">
<span style="font-size: 1.05rem">{{ chair.chair }}</span><br>
{% for member in chair.members %}
<b>{% assign names = member.name | sort: 'a_sort' %}</b>
{% for name in names %}
<br><b>{{ name.n }} {{ name.a }}</b><br>
{% endfor %}
<br>{{ member.organization }}<br><br>
{% endfor %}
</div>
{% endfor %}

<h5 style="padding: 0.2rem;color:white; background-color: #550000; border-radius: 5px"><i class="fa fa-users mr-3"></i> <b>Comité Ejecutivo</b></h5>



{% assign members_ejecutivo = site.data.comite_ejecutivo  %}
<div style="font-size: 0.9rem; padding-top: 1.5rem; padding-bottom: 1.5rem;">
{% for member in members_ejecutivo %}

<b>{{ member.name }} {{ member.surname }}</b><br>
<br>{{ member.organization }}<br><br><br>
{% endfor %}
</div>



<h5 style="padding: 0.2rem;color:white; background-color: #e3041e; border-radius: 5px"><i class="fa fa-users mr-3"></i> <b>Comité de Programa de Formación e Innovación Educativa</b></h5>
{% assign chairs = site.data.comite_programa_formacion %}
{% for chair in chairs %}
<div style="font-size: 0.9rem; padding-top: 1.5rem; padding-bottom: 1.5rem;">
<span style="font-size: 1.05rem">{{ chair.chair }}</span><br>
{% for member in chair.members %}
{% assign names = member.name | sort: 'a_sort' %}
{% for name in names %}
<br><b>{{ name.n }} {{ name.a }}</b><br>
{% endfor %}
<br>{{ member.organization }}<br><br>
{% endfor %}
</div>
{% endfor %}



</div>
<div class="column" style="background-color: #F5F5F5;box-shadow:0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);">





<h5 style="padding: 0.2rem;color:white; background-color: #e3041e; border-radius: 5px"><i class="fa fa-users mr-3"></i> <b>Comité de Programa Científico</b></h5>
{% assign chairs = site.data.comite_programa_cientifico %}
{% for chair in chairs %}
<div style="font-size: 0.9rem; padding-top: 1.5rem; padding-bottom: 1.5rem;">
<span style="font-size: 1.05rem">{{ chair.chair }}</span><br>
{% for member in chair.members %}
{% assign names = member.name | sort: 'a_sort' %}
{% for name in names %}
<br><b>{{ name.n }} {{ name.a }}</b><br>
{% endfor %}
<br>{{ member.organization }}<br><br>
{% endfor %}
</div>
{% endfor %}


<h5 style="padding: 0.2rem;color:white; background-color: #e3041e; border-radius: 5px"><i class="fa fa-users mr-3"></i> <b>Comité de Transferencia Tecnológica</b></h5>
{% assign chairs = site.data.comite_transferencia_tecnologica %}
{% for chair in chairs %}
<div style="font-size: 0.9rem; padding-top: 1.5rem; padding-bottom: 1.5rem;">
<span style="font-size: 1.05rem">{{ chair.chair }}</span><br>
{% for member in chair.members %}
{% assign names = member.name | sort: 'a_sort' %}
{% for name in names %}
<br><b>{{ name.n }} {{ name.a }}</b><br>
{% endfor %}
<br>{{ member.organization }}<br><br>
{% endfor %}
</div>
{% endfor %}



<!--
{% assign members_investigacion = site.data.comite_programa_investigacion | sort: 'surname_sort' %}
{% for member in members_investigacion %}


 
<div style="font-size: 0.9rem; padding-top: 1.5rem; padding-bottom: 1.5rem;">
<b>{{ member.name }} {{ member.surname }}</b><br><br>
{{ member.organization }}
</div>

{% endfor %}
-->



</div>
</div> 
<!--</div>-->
