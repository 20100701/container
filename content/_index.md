+++
title = "Conteneurisation"
+++

<!-- Slide TITLE -->
<!--: .wrap .text-landing ..aligncenter -->
<!--: .text-Virgil -->
Alexandre Linte / Gaëtan Allain
<br><br>
# **Conteneurisation** <br>
2021 - 2022<br>

---
<!-- Slide ABOUT -->
<!--: .wrap -->
<!--: .text-Virgil -->
{{< div class="content-left" >}}

#### Avant-propos
<small>
*Ce contenu a pour objectif de faire découvrir les concepts de la conteneurisation. Certains aspects sont simplifiés dans le but de rester compréhensible par un public voulant appréhender ce sujet sans en devenir des experts.*
</small>
<br><br><br>
#### Objectif
<small>
Ce contenu doit permettre aux étudiants d'appréhender les concepts de la conteneurisation ainsi que les solutions techniques misent en œuvre.<br>
Il sert donc de support pour un module d'enseignement de la conteneurisation aussi bien pour les parties théorique que pratique. Il limite au maximum le temps passé sur la phase de déploiement des environnements afin de laissé le plus de temps possible à la compréhension de la conteneurisation et aux échanges entre étudiants et formateurs.
</small>
{{< /div >}}


<figure class="content-right">
  <img alt="Screenshot" src="https://images.unsplash.com/photo-1519452635265-7b1fbfd1e4e0?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=934&q=80">
</figure>


---
<!-- Slide 3 -->
<!--: .wrap -->
<!-- : .text-Virgil -->
{{< div class="content-left" >}}
### Qu'est ce qu'un conteneur ?
Un conteneur est un package logiciel (application) qui contient l'**ensemble des fichiers** (<small><a href=https://en.wikipedia.org/wiki/Everything_is_a_file>*Everything is a file*</a></small>) qui lui permettent de fonctionner de manière isolée, en autonomie.<br>
C'est aussi un **processus** (ou ensemble de processus) **isolé** du reste du système, il posséde ses propres ressources : cpu, ram, réseau, sytème de fichiers, ...<br>
Il est construit à partir d'une **image de conteneur**.<br>
<br><br><br><br><br>
{{% fontawesome book-reader %}}  <small>Il est possible d'avoir un aperçu de l'histoire des conteneurs <a href=https://blog.aquasec.com/a-brief-history-of-containers-from-1970s-chroot-to-docker-2016>ici</a>.</small>
{{< /div >}}

<figure class="content-right">
  <img alt="Screenshot" src="https://20100701.github.io/container/static/images/container.svg">
</figure>

---
<!-- Slide 4 -->
<!--: .wrap -->
<!-- : .text-Virgil -->
### Qu'est-ce que la conteneurisation ?
La conteneurisation est un type de virtualisation d'application au niveau du système d'exploitation.<br>
Cela permet de lancer plusieurs conteneurs (applications) isolés les uns des autres sur une même machine hôte.<br>
La conteneurisation est particulièrement bien adaptée au concept de micro-services, elle permet aussi de gérer la consommation des ressources au plus juste.<br>
<br>
Il existe plusieurs solutions de conteneurisation, voici quelques exemples :<br>
- <a href=https://linuxcontainers.org/lxc/introduction/>LXC</a> et <a href=https://linuxcontainers.org>plus</a><br>
- <a href=https://www.docker.com/>Docker</a><br>
- <a href=https://getfedora.org/en/coreos?stream=stable>Fedora CoreOS</a><br>
- <a href=https://openvz.org/>Open VZ</a><br>
- <a href=https://kubernetes.io/fr/>Kubernetes</a> (aka K8S)<br>
- <a href=https://mesos.apache.org/>Mesos</a><br>

---
<!-- Slide 5 -->
<!--: .wrap -->
<!-- : .text-Virgil -->
### Conteneur || Machine Virtuelle 1/2
Les conteneurs et les machines virtuelles ne sont pas en concurrence, où ne devraient pas l'être. Ce sont deux solutions différentes dans la boîte à outil du concepteur d'application.
Par contre il est vrai que les conteneurs prennent une partie significative des *workloads* qui hier tournaient sur des machines virtuelles.

##### Critères de choix
Le choix d'utiliser une Machine Virtuelle (VM) ou un conteneur se fait en fonction de certains critères, voici quelques exemples :<br>
- consommation de ressource (ex : cpu, ram)<br>
- élasticité<br>
- portabilité<br>
- architecture applicative (ex : distribuée)<br>
- facilité d'intégration
- cycle de vie de l'application

<small>*Note : Au sein d'une entreprise l'utilisation de l'une ou l'autre de ces solutions peut aussi être liée à la stratégie de l'entreprise.*</small>

---
<!-- Slide 6 -->
<!--: .wrap -->
<!-- : .text-Virgil -->
### Conteneur || Machine Virtuelle 2/2
<!--: .flexblock gallery -->
- {{< gallery title="vm" href="https://20100701.github.io/container/static/images/vm.svg" src="https://20100701.github.io/container/static/images/vm.svg" >}}{{< /gallery >}}

- {{< gallery title="container" href="https://20100701.github.io/container/static/images/container.svg" src="https://20100701.github.io/container/static/images/container.svg" >}}{{< /gallery >}}


---
<!-- Slide 7 -->
<!--: .wrap -->
### Quelles sont les limites de la conteneurisation ?

##### Ecosystème
Aujourd'hui, l'écosystème autour des solutions de conteneurisation commence à peine à se stabiliser, certains arrivent à matûrité (fiabilité, fonctionnalités), mais du fait du grand nombre d'acteurs du marché impliqués cela devrait arriver dans les années à venir. 

###### Portabilité
Tout comme les VM, il existe une limitation d'usage en fonction du système d'exploitation. Un conteneur Linux ne peut être directement utiliser sur une machine hôte Windows. 

##### Sécurité
Tout comme les VM, il est possible d'exploiter des failles pour prendre la main sur le système hôte en cas de compromission d'un conteneur.

##### Exploitation de la solution
La solution de conteneurisation est aussi complexe à gérer que le sont les solutions de virtualisation.

{{% fontawesome bullhorn %}}<small> la conteneurisation ne résoud pas tous les problèmes de l'informatique ! </small>

---
<!-- Slide 8 -->
<!--: .wrap .text-landing bg=bg-black bg=left bgimage=https://cdn.pixabay.com/photo/2018/05/07/22/32/microphone-3381837_960_720.jpg -->
# **QUESTION ?**

---
<!-- Slide 9 -->
<!--: .wrap .text-landing ..aligncenter -->
# **Docker** <a href=https://www.docker.com>{{% fontawesome docker %}} </a>

---
<!-- Slide 10 -->
<!--: .wrap .card-50 .bg-white-->
<!--: .flexblock content -->
### Qu'est-ce que Docker ?
<a href=https://www.docker.com>Docker</a> est une solution **Open Source** d'hébergement de conteneur (aka container) **multi-plateformes**.
Elle permet de mettre en oeuvre des conteneurs Docker en s'appuyant sur le **noyau Linux**. Docker utilise plusieurs fonctionnalités du noyau Linux pour garantir l'isolation entre les conteneurs Docker.

<!--: .flexblock gallery -->
- {{< gallery title="Docker Kernel Linux" href="https://upload.wikimedia.org/wikipedia/commons/thumb/0/09/Docker-linux-interfaces.svg/1920px-Docker-linux-interfaces.svg.png" src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/09/Docker-linux-interfaces.svg/650px-Docker-linux-interfaces.svg.png" >}}{{< /gallery >}}

---
<!-- Slide 11 -->
<!--: .wrap -->
### Docker, les premiers pas  {{% fontawesome walking %}}
<small>Note : la doc officielle de Docker est bien faite ... </small><a href=https://docs.docker.com>{{% fontawesome book-open %}}</a>

<!--: .flexblock gallery -->
- {{< gallery title="use Docker" href="https://docs.docker.com/engine/images/architecture.svg" src="https://docs.docker.com/engine/images/architecture.svg" >}}{{< /gallery >}}

---
<!-- Slide 12 -->
<!--: .wrap -->
#### Docker image <a href=https://docs.docker.com/engine/reference/commandline/image/>{{% fontawesome book-open %}}</a>
Les images Docker sont des templates d'application (au sens large du terme) au format Docker, elles contiennent l'ensemble des instructions permettant à l'application de fonctionner sur le **Docker Engine**. Tous les **Docker containers** sont créés à partir d'une **Docker image**.

Les images sont mises à disposition à travers de **Registry**, celle qui fait référence pour Docker est le <a href=https://hub.docker.com/search?q=&type=image>**Docker Hub**</a>.

#### Dockerfile <a href=https://docs.docker.com/engine/reference/builder>{{% fontawesome book-open %}}</a>
Comme son nom l'indique, **Dockerfile** est un fichier, il contient l'**ensemble des instructions** permettant au **Docker Engine** de créer une **Docker image**.

~~~dockerfile
# Exemple (minimaliste) d'un Dockerfile
FROM busybox
COPY somefile.txt .
RUN cat /somefile.txt
~~~
<small>Les *best practices* relatives à la rédaction de Dockerfile sont <a href=https://docs.docker.com/develop/develop-images/dockerfile_best-practices>ici</a>.</small>

---
<!-- Slide 13 -->
<!--: .wrap .text-landing ..aligncenter bg=bg-black bg=aligncenter bgimage=https://raw.githubusercontent.com/docker-library/docs/471fa6e4cb58062ccbf91afc111980f9c7004981/swarm/logo.png -->
# **Swarm : Docker clustering**

---
<!-- Slide 14 -->
<!--: .wrap -->
### Swarm <a href=https://docs.docker.com/engine/swarm/key-concepts/>{{% fontawesome book-open %}} </a>
**Swarm** (aka swarmkit) est un développement distinct de Docker. Swarm permet la mise en <a href=https://en.wikipedia.org/wiki/Computer_cluster>cluster</a> de **Docker engines**.<br>
Les rôles confiés à Swarm sont donc la **gestion** et **l'orchestration** des différents *Docker engines* qui composent le cluster.<br>

Il est courant d'appeler **noeuds** (aka nodes) les éléments qui composent un cluster.<br>
Dans le contexte Swarm les noeuds sont des instances de *Docker engine*, ils peuvent être de 2 types **manager** ou **worker**.

###### Manager nodes
Les noeuds *manager* sont des instances de *Docker engine* assurent la **gestion** du cluster ainsi que l'**orchestration** des *workloads* (conteneurs).
Les noeuds *manager* permettent d'intéragir avec le cluster. 

###### Worker nodes
Les *Docker containers* sont exécutés sur les noeuds *worker*.

<!--: .flexblock gallery -->
- {{< gallery title="swarm cluster" href="https://20100701.github.io/container/static/images/swarm.svg" src="https://20100701.github.io/container/static/images/swarm.svg" >}}{{< /gallery >}}

---
<!-- Slide 15 -->
<!--: .wrap -->




---
<!-- Slide END -->
<!--: .wrap .text-landing bg=bg-white bg=aligncenter bgimage=https://images.unsplash.com/photo-1583791031153-d55e79f7f115?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1867&q=80 -->
# **Thank you for your attention**