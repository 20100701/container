+++
title = "Container Overview"
+++

<!-- Slide 1 -->
<!--: .wrap bg=bg-black bg=aligncenter bgimage=https://images.unsplash.com/photo-1565264316550-a1811f0c4c75?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=975&q=80 -->

{{< div class="content-center" >}}
# **Container Overview**  
[{{% fontawesome github %}} Github](https://20100701.github.io/container/)
{{< /div >}}

---
<!-- Slide 2 -->
{{< div class="content-left" >}}

#### Avant-propos
<small>
*Ce contenu a pour objectif de faire découvrir les concepts de la conteneurisation. Certains aspects sont simplifiés dans le but de rester compréhensible par un public voulant appréhender ce sujet sans en devenir des experts.*
</small>

#### Contexte
<small>
Ce contenu a été créé pour les étudiants de la licence <a href="https://uniform.unicaen.fr/catalogue/formation/licences-pro/5236-licence-pro-metiers-informatique---administration-securite-systemes-et-reseaux-parcours-audit-securite-reseaux-sys-info?s=iut-caen&r=1291046129051">Audit et Sécurité des Réseaux et des Systèmes d'Information</a> (aka ASRSI) de l'<a href="http://www.unicaen.fr/">Université de Caen</a>.
</small>

#### Objectif
<small>
Ce contenu doit permettre aux étudiants d'appréhender les concepts de la conteneurisation ainsi que les solutions techniques misent en œuvre.<br>
Il sert donc de support pour un module d'enseignement de la conteneurisation aussi bien pour les parties théoriques que pratiques. Il limite au maximum le temps passé sur la phase de déploiement des environnements afin de laissé le plus de temps possible à la compréhension de la conteneurisation et aux échanges entre étudiants et formateurs.
</small>
{{< /div >}}


<figure class="content-right">
  <img alt="Screenshot" src="https://images.unsplash.com/photo-1519452635265-7b1fbfd1e4e0?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=934&q=80">
</figure>

---
<!-- Slide 3 -->
<!--: .wrap -->
### Qu'est ce qu'un conteneur ?
Un conteneur est un package logiciel (application) qui contient l'**ensemble des fichiers** (<small><a href=https://en.wikipedia.org/wiki/Everything_is_a_file>*Everything is a file*</a></small>) qui lui permettent de fonctionner de manière isolée, en autonomie.<br>
C'est aussi un **processus** (ou ensemble de processus) **isolé** du reste du système, il posséde ses propres ressources : cpu, ram, réseau, sytème de fichiers, ...
Il est construit à partir d'une **image de conteneur**.<br>

<!--: .flexblock gallery -->
- {{< gallery title="2020" href="https://20100701.github.io/container/static/images/archi-container.svg" src="https://20100701.github.io/container/static/images/archi-container.svg" >}}{{< /gallery >}}


{{% fontawesome book-reader %}}<small>Il est possible d'avoir un aperçu de l'histoire des conteneurs en cliquant <a href=https://blog.aquasec.com/a-brief-history-of-containers-from-1970s-chroot-to-docker-2016>ici</a>.</small>

---
<!-- Slide 4 -->
<!--: .wrap -->
#### Comment fonctionne la conteneurisation ?




---
<!-- Slide X -->
<!--: .wrap -->
### Conteneur vs Machine Virtuelle

---
<!-- Slide 5 -->
<!--: .wrap -->
### Pourquoi utiliser les conteneurs ?

Comme ils n'incluent pas de systèmes d'exploitation complets, les conteneurs ne nécessitent que des ressources de calcul minimales, et leur installation est rapide et facile. Cette efficacité leur permet d'être déployés en clusters, avec des conteneurs individuels intégrant des composants d'applications complexes. Le fait de séparer les composants dune 'application en différents conteneurs permet aux développeurs d'actualiser ces composants sans réorganiser l'application tout entière.

multiples systèmes d’exploitation, quels qu’ils soient. Ils garantissent que leur contenu est identique au départ et à l’arrivée, et qu’il est sécurisé, grâce à leur mise en isolation.

Ils servent à minimiser la complexité liée à la configuration et à l’administration applicatives, à accélérer les cycles de développement et de production applicatifs, et, grâce à leur flexibilité et à leur portabilité, ils constituent l’une des briques qui permettent de faire de l’« infrastructure as a service », c’est-à-dire d’automatiser les infrastructures IT.

La conteneurisation propose une manière de virtualiser des ressources de manière légère, avec une isolation garantie par le système d’exploitation. Ces ressources sont ainsi plus facilement portables d’un système à un autre. C’est un puissant accélérateur de développement d’applications.

---
<!-- Slide 6 -->
<!--: .wrap -->
### Quelles sont les limites de la conteneurisation ?
En matière de conteneurisation, les outils arrivent petit à petit à maturité. C’est-à-dire que la conteneurisation et le support sur lequel elle s’appuie commencent (à l’intérieur du noyau Linux) à être complètement fiables. On n’observe plus les failles qui permettaient, il y a encore quelques années, de briser les protections et de s’introduire à l’intérieur d’un conteneur pour accéder frauduleusement aux ressources de la machine. Aujourd’hui, ce n’est plus possible parce que le code utilisé est abouti et que les ops sont bien mieux formés pour limiter les possibilités d’intrusion. Par exemple en limitant les droits sur les applications.

Cependant, pour les orchestrateurs de conteneurs, il existe encore des limitations. Par exemple en matière de gestion de grands volumes de données, il reste des progrès à faire pour l’intégration avec les fournisseurs de cloud. Par ailleurs, de nombreuses applications à migrer vers le cloud ne peuvent pas bénéficier des avantages de l’orchestration des conteneurs pour le passage à à l’échelle et la portabilité. Il faudrait les réécrire pour les adapter à cette nouvelle approche, mais cela demanderait trop de temps.

---
<!-- Slide N -->
<!--: .wrap bg=bg-black bg=left bgimage=https://cdn.pixabay.com/photo/2018/05/07/22/32/microphone-3381837_960_720.jpg -->
# QUESTION ?

---
<!-- Slide X -->
<!--: .wrap .text-landing -->
# Docker <a href=https://www.docker.com>{{% fontawesome docker %}} </a>






