+++
title = "Container Overview"
+++

<!-- Slide 1 -->
<!--: .wrap bg=bg-black bg=aligncenter bgimage=https://images.unsplash.com/photo-1565264316550-a1811f0c4c75?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=975&q=80 -->

{{< div class="content-center" >}}
# **Container Overview**  
[{{% fontawesome github %}}Github](https://20100701.github.io/container/)
{{< /div >}}



---
<!-- Slide 2 -->
{{< div class="content-left" >}}
### Avant-propos
*Ce contenu a pour objectif de faire découvrir les concepts de ce que l'on appelle le "Big Data". Certains aspects sont simplifiés dans le but de rester compréhensible par un public voulant appréhender ce sujet sans en devenir des experts.*

### Contexte
Ce contenu a été créé pour les étudiants de la licence <a href="https://uniform.unicaen.fr/catalogue/formation/licences-pro/5236-licence-pro-metiers-informatique---administration-securite-systemes-et-reseaux-parcours-audit-securite-reseaux-sys-info?s=iut-caen&r=1291046129051">Audit et Sécurité des Réseaux et des Systèmes d'Information</a> (aka ASRSI) de l'<a href="http://www.unicaen.fr/">Université de Caen</a>.

### Objectif
Ce contenu doit permettre aux étudiants d'appréhender les concepts du Big Data ainsi que les solutions techniques misent en œuvre.<br>
Il sert donc de support pour un module d'enseignement du Big Data aussi bien pour les parties théoriques que pratiques. Il limite au maximum le temps passé sur la phase de déploiement des environnements afin de laissé le plus de temps possible à la compréhension du Big Data et aux échanges entre étudiants et formateurs.
{{< /div >}}


<figure class="content-right">
  <img alt="Screenshot" src="https://images.unsplash.com/photo-1519452635265-7b1fbfd1e4e0?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=934&q=80">
</figure>

---
<!-- Slide 3 -->
<!--: .wrap -->
# Big Data, qu'est-ce que c'est ?

## Une problématique
C'est l'un des plus grands défis des années 2010-2030 pour le monde de l'IT mais aussi et surtout pour l'ensemble de la société (citoyens, états, entreprises, ...). Ce défi est aussi bien technique que sociétale.

En effet, avec la capacité à récolter et effectuer de traitement sur des quantités de donnée de plus en plus importante, les questions autour de la propriété de ces données et de leur utilisation se posent aujourd'hui. L'Europe a par exemple déjà légiféré sur le sujet en votant le <A href="https://fr.wikipedia.org/wiki/Règlement_général_sur_la_protection_des_données">Règlement Général sur la Protection des Données</a> (aka RGPD), le texte est disponible <a href="https://eur-lex.europa.eu/legal-content/FR/TXT/?uri=CELEX:32016R0679">ici</a>.

## Le principe des 3 V
Nous n'avons pas attendu l'avènement du terme "Big Data" pour récolter et effectuer du traitement sur des données. Ce qui change avec le "Big Data" ce sont essentiellement trois caractéristiques liées aux capacités de traitement et à la récolte de donnée : <br>
-  **le volume** : le nombre de donnée créé ne cesse de croitre<br>
-  **la vélocité** : la fréquence à laquelle les données sont créées/récoltées/partagées est de plus en plus élevée<br>
-  **la variété** : les données sont de diverses formes (brutes, non-structurées, structurées, semi-structurées)<br>

---
<!-- Slide 4 -->
<!--: .wrap -->
# Quelques chiffres 
Pour entrapercevoir le monde du Big Data voici quelques chiffres :<br>
<small>Note : il y a 525 600 minutes dans une année</small>

<!--: .flexblock gallery -->
- {{< gallery title="2020" href="https://20100701.github.io/bigdata/static/images/internet-minute-2020.jpg" src="https://20100701.github.io/bigdata/static/images/internet-minute-2020.jpg" >}}{{< /gallery >}}
- {{< gallery title="2019" href="https://20100701.github.io/bigdata/static/images/internet-minute-2019.jpg" src="https://20100701.github.io/bigdata/static/images/internet-minute-2019.jpg" >}}{{< /gallery >}}
- {{< gallery title="2018" href="https://20100701.github.io/bigdata/static/images/internet-minute-2018.jpg" src="https://20100701.github.io/bigdata/static/images/internet-minute-2018.jpg" >}}{{< /gallery >}}

---
<!-- Slide 5 -->
<!--: .wrap -->
## Un écosystème
Avec les années, l'écosystème du Big Data est devenu de plus en plus important et il est maintenant associé à celui de l'intelligence artificielle, comme présenté ci-dessous.

<!--: .flexblock gallery -->
- {{< gallery title="landscape" href="https://20100701.github.io/bigdata/static/images/landscape.png" src="https://20100701.github.io/bigdata/static/images/landscape.png" >}}{{< /gallery >}}

---
<!-- Slide 6 -->
<!--: .wrap -->

## Une tendance qui s'accélère
La croissance du Big Data n'est pas prête de s'arrêter et plusieurs facteurs vont l'aider en cela :<br>
- l'IPv6 : le déploiement de l'IPv6 dans les réseaux opérateurs et d'entreprises va permettre de connecter 667 millions de milliards d'appareils à Internet sur chaque millimètre carré de la surface terrestre.<br>
- le coût du stockage : nous sommes passé d'un coût du Go en 2000 de 10$ à 0,03$ en 2015 soit une baisse de 99,7% sur 15 ans.<br>
- le nombre d'internaute : en 2018, 3,8 milliards d'humain utilisent Internet<br>
- le débits des réseaux : les capacités des réseaux (LAN, MAN, WAN, câbles sous-marins, liaisons satellites) augmentent en permanence<br>
- les domaines utilisant des objets connectés : de plus en plus de domaine utilisent des objets connectés comme le médical, la domotique, les télécommunications, la finance, l'agriculture, … L'illustration ci-dessous montre bien la croissance rapide du domaine de l'IoT (Internet of Things), ce qui permet de comprendre l'accélération de la création et la récolte des données.<br>


![croissance IoT](https://www.cisco.com/c/dam/en_us/about/security/images/csc_child_pages/white_papers/iot-figure1.jpg)


---
<!-- Slide 7 -->
<!--: .wrap -->
### Exemples d'acteur du Big Data
Dans les principaux acteurs du Big Data, il y a des acteurs du monde de l'IT mais aussi des sociétés dont le cœur de métier est tout autre.

Parmi les leaders du domaine, il y a Google, Apple, Facebook, Yahoo!, Amazon , Microsoft mais aussi Netflix, Tesla, Uber, AirBnB ... 

### Exemples de cas d'usage
Il y a beaucoup d'exemple de cas d'usage Big Data, ceux qui sont listés ci-dessous ont été choisis car ils ne sont pas liés à des entreprises du monde de l'IT. Ils montrent que dès qu'une entreprise détient un grand nombre de donnée, elle peut en tirer un profit grâce au Big Data, quel que soit son secteur d'activité.<br>
<small>
<br>**Suivi épidémiologique**<br>
Grâce à l'Open Data il est possible de suivre l'évolution de la pandémie de covid-19. (<a href=https://covidtracker.fr>site</a>)
<br>**Sauvons les Livebox**<br>
Orange a mis en place en 2016 un scénario Big Data lui permettant de limiter le nombre de Livebox foudroyée. (<a href=https://datascience.wp.imt.fr/2016/04/11/livebox-foudroyee-en-spark>article</a>)
<br>**Vue client 360°**<br>
T-Mobile a mis en place grâce au Big Data une vue client 360° afin de limiter la perte de client. (<a href=https://datafloq.com/read/t-mobile-usa-cuts-downs-churn-rate-with-big-data/512>article</a>)
<br>**Publicité ciblée**<br>
Starbuck a mis en place un système de publicité ciblée grâce aux traitements effectués sur les données de ses clients. (<a href=https://www.forbes.com/sites/bernardmarr/2018/05/28/starbucks-using-big-data-analytics-and-artificial-intelligence-to-boost-performance/#4b0acd0165cd>article</a>)
<br>**Personnalisation des recommandations**<br>
Spotify utilise le Big Data pour proposer à ses clients les morceaux de musique les plus pertinents en fonction de leur goût. (<a href=https://labs.spotify.com/2016/08/07/commodity-music-ml-services/>article</a>)
<br>**Sur de bons rails**<br>
Union Pacific gère les actes de maintenance préventive à l'aide du Big Data et des objets connectés, ce qui a réduit le risque de "déraillement" de ces trains et augmenté la disponibilité des voies. (<a href=https://datafloq.com/read/union-pacific-railroad-turned-industrial-internet-/365>article</a>)
<br>**Le même jus d'orange**<br>
Coca Cola mixe des données satellite, de la météo, des récoltes d'orange et beaucoup d'autres pour s'assurer que le goût de leur jus d'orange sera toujours le même quelque soit la période de l'année. (<a href=https://www.forbes.com/sites/bernardmarr/2017/09/18/the-amazing-ways-coca-cola-uses-artificial-intelligence-ai-and-big-data-to-drive-success/#58b6a1d078d2>article</a>)
<br>**Risque d'agression**<br>
Rabobank utilise les données de ses distributeurs de billet et d'autres (météo, position, ...) pour calculer le risque de se faire agresser en retirant de l'argent. (<a href=https://datafloq.com/read/with-proof-of-concepts-rabobank-learned-valuable-b/503>article</a>)
<br>**Assistant agricole**<br>
John Deere permet aux agriculteurs mesurer différentes activités afin de les aider à prendre les décisions. (<a href=https://www.terre-net.fr/materiel-agricole/tracteur-quad/article/a-quoi-servent-les-solutions-connectees-john-deere-concretement-207-146778.html>article</a>)
</small>

---
<!-- Slide 8 -->
<!--: .wrap -->
# Big data, une ( r )évolution technique
L'essor du Big Data a entrainé une ( r )évolution dans la façon dont les datacenters étaient gérés. Les infrastructures techniques sur lesquelles fonctionnent les solutions de Big Data comportent de très nombreuses machines physiques le déploiement et la gestion de toutes ces machines est un vrai défi.

La **standardisation** et l'**automatisation** sont deux des aspects les plus importants lorsqu'il s'agit d'opérer, de construire ou de faire évoluer rapidement une solution de Big Data afin de limiter les erreurs humaines et de réduire les coûts.

Pour faciliter la mise en œuvre de ces infrastructures Big Data, toutes les **machines sont identiques**, cela permet de **rationnaliser leur gestion** (ex : remplacement en cas de panne). Du fait de leur nombre, ces machines sont choisis pour limiter la consommation d'énergie (alimentation électrique, climatisation, ...) car la ce poste de dépense est le plus important dans un datacenter.

---
<!-- Slide 9 -->
<!--: .wrap -->
# Les clusters qui passent à l'échelle (hyperscale)
La notion de cluster est connue dans le monde informatique depuis de très nombreuses années. Il existe pléthore de solution technique qui fonctionne avec des clusters, souvent constituées de 2 à quelques dizaines de machine. 

Mais dans l'univers du Big Data, les clusters peuvent atteindre plusieurs milliers de machine, c'est pour cela que la mention "qui passent à l'échelle" est importante. De par leur taille les clusters Big Data doivent couvrir l'ensemble des exigences suivantes :<br>
- **Évolutivité (Scalability)** : capacité à pouvoir croître<br> 
- **Élasticité (Elasticity)** : capacité à être redimensionné sans arrêt de service<br>
- **Cohérence (Constitency)** : capacité à ne pas perdre/altérer les données/traitements<br>
- **Résilience (Resilient)** : capacité à pouvoir perdre un ou plusieurs éléments sans impact<br>
- **Disponibilité (Availibility)** : capacité à avoir un taux de disponibilité proche de 100%<br>
- **Distribution (Distributive)** : capacité à pouvoir être déployé dans plusieurs racks/zones/sites distants<br>

---
<!-- Slide 10 -->
<!--: .wrap -->
# Le réseau
Un cluster Big Data a besoin de s'appuyer sur un réseau afin de pouvoir **récolter** les données et les **échanger** entre les différents nœuds du cluster. Les clusters Big Data manipulent de **très grande quantité de donnée**, il est donc facile de concevoir que la capacité du réseau à pouvoir transporter rapidement ces données est un enjeu majeur.
Pour répondre à ce besoin l'architecture des réseaux au sein des datacenters évolue pour passer d'un modèle "3 tiers" à un modèle "Spine-leaf".

---
<!-- Slide 11 -->
<!--: .wrap -->

## Architecture réseau "3 tiers"
Comme son nom l'indique ce modèle est composé de **3 étages de composant réseau** (switch). Cette architecture n'est pas adaptée aux exigences du Big Data. En effet, si les serveurs représentent les différents nœuds du cluster, le transfert de donnée entre ces nœuds va **transiter jusqu'au "Core switch"**. De plus, un seul chemin réseau est actif pour atteindre une destination (les liens sont en mode **actif/passif**). Du fait du volume de donnée manipulé par un cluster Big Data, cette architecture augmente le risque de congestion du réseau ce qui nuira à la performance du cluster Big Data. 

{{< div class="content-center" >}}
![architecture 3 tiers](https://20100701.github.io/bigdata/static/images/3tiers.png)
{{< /div >}}

---
<!-- Slide 12 -->
<!--: .wrap -->
## Architecture réseau "Spine-leaf"
Cette architecture est composée de **2 étages de composant réseau** (switch). En plus de la diminution du nombre de composant, l'intérêt de ce modèle est qu'il permet d'utiliser l'ensemble des liens réseaux en même temps (**actif/actif**).
Le résultat est qu'il y a plusieurs chemins réseaux possible (**+ de débit**) entre 2 nœuds et ils sont plus courts (**- de latence**).
Il est à noter un autre avantage, il est très facile d'augmenter le nombre de switch. En effet, avec cette topologie l'ajout de switch augmente le nombre de chemin réseau possible est donc diminue le risque de congestion.

{{< div class="content-center" >}}
![spine leaf architecture](https://20100701.github.io/bigdata/static/images/spine_leaf_network.png)
{{< /div >}}

---
<!-- Slide 13 -->
<!--: .wrap bg=bg-black bg=left bgimage=https://cdn.pixabay.com/photo/2018/05/07/22/32/microphone-3381837_960_720.jpg -->
# QUESTION ?

---
<!-- Slide 14 -->
<!--: .wrap bg=bg-black bg=left bgimage=https://yubigeek.s3.eu-west-3.amazonaws.com/615/responsive-images/3394fcd0-21eb-411b-83d0-b618bcc65dac___media_library_original_1791_1266.jpeg -->

---
<!-- Slide 15 -->
<!--: .wrap -->

# Apache Hadoop, c'est quoi ?
Il existe un grand nombre de solution de Big Data, nous avons choisi de commencer par étudier la solution <a href=https://hadoop.apache.org/>Hadoop</a> car c'est l'une des solutions les plus utilisées (quelques exemples d'utilisation d'Hadoop <a href=https://cwiki.apache.org/confluence/display/HADOOP2/PoweredBy>ici</a>).

### ![logo Hadoop](https://hadoop.apache.org/elephant.png) La solution Hadoop
Apache Hadoop est une solution écrite en Java qui a pour but de faciliter les traitements distribués sur de grande quantité de donnée. Elle est composée de plusieurs modules (common, hdfs, yarn, mapreduce, ...).Pour cela elle s'appuie sur une architecture en cluster qui passent à l'échelle (hyperscale).

Mais Hadoop n'est pas composé d'un cluster mais en fait de deux clusters qui fonctionnent en parallèle :<br>
- Hadoop Distributed File System (**HDFS**) : pour gérer les ressources de stockage (disk) et les données déposées dans le système de fichier.<br>
- Yet Another Ressource Negociator (**YARN**) : pour gérer les ressources de calcul (cpu + ram) et les traitements qui s'exécutent sur le cluster.<br>

### Deux clusters indépendants
Pourquoi dit-on qu'**HDFS et YARN fonctionnent indépendamment l'un de l'autre** ?
Parce qu'il est possible d'utiliser uniquement HDFS, par exemple, il est possible de stocker des données sur HDFS pour des besoins d'archivage, sans jamais avoir besoin d'effectuer des traitements YARN sur ces données. Inversement, les traitements exécutés sur YARN peuvent ne pas avoir besoin d'utiliser des données stockées sur HDFS comme les calculs mathématiques (ex : le calcul des décimales de PI).

---
<!-- Slide 16 -->
<!--: .wrap -->
# Écosystème Hadoop
Hadoop fait parti d'un écosystème Big Data ou il existe énormément de solution technique. L'illustration ci-dessous propose la vision de Mercy (Ponnupandy) Beckham de cet écosystème.

![écosystème Hadoop](https://mydataexperiments.files.wordpress.com/2017/04/hadoop-ecosystem.png)
<br><small>*crédits : Mercy (Ponnupandy) Beckham (2017)*</small>

---
<!-- Slide 17 -->
<!--: .wrap -->

# HDFS en quelques mots
<A href="https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html">HDFS</A> est un système de fichiers distribué, extensible et portable développé par Hadoop à partir du <A href="https://fr.wikipedia.org/wiki/Google_File_System">GoogleFS</A>.  
Écrit en Java, il a été conçu pour stocker de très gros volumes de données sur un grand nombre de machines équipées de disques durs banalisés. Il permet l'abstraction de l'architecture physique de stockage, afin de manipuler un système de fichiers distribué comme s'il s'agissait d'un disque dur unique.

### Les composants HDFS
Une architecture système de fichier HDFS repose sur deux types de composants majeurs : le **namenode** et le **datanode**.

#### Namenode
Ce composant gère l'espace de noms, l'arborescence du système de fichiers et les métadonnées des fichiers et des répertoires. Il centralise la localisation des blocs de données répartis dans le cluster. 

#### Datanode
Ce composant stocke et restitue les blocs de données. Lors du processus de lecture d'un fichier, le NameNode est interrogé pour localiser l'ensemble des blocs de données. Pour chacun d'entre-eux, le NameNode renvoie l'adresse du DataNode le plus accessible, c'est-à-dire le DataNode qui dispose de la plus grande bande passante. Les DataNodes communiquent de manière périodique au NameNode la liste des blocs de données qu'ils hébergent. Si certains de ces blocs ne sont pas assez répliqués dans le cluster, l'écriture de ces blocs s'effectue en cascade par copie sur d'autres.

---
<!-- Slide 18 -->
<!--: .wrap -->
## HDFS : opération d'écriture

![hdfs-WRITE](https://20100701.github.io/bigdata/static/images/hdfs-WRITE.png)

<br><small>*Note : une fois l'opération d'écriture effectuée, le Namenode mets à jour les metadata après avoir interroger les différents Datanodes. Ce mécanisme se déroule régulièrement ce qui permet au Namenode de garantir la cohérence des données stockées dans le système de fichier HDFS et leurs emplacements.*</small>

---
<!-- Slide 19 -->
<!--: .wrap -->
## HDFS : opération de lecture 

![hdfs-READ](https://20100701.github.io/bigdata/static/images/hdfs-READ.png)

---
<!-- Slide 20 -->
<!--: .wrap -->
# Yarn en quelques mots
<A href="https://hadoop.apache.org/docs/current/hadoop-yarn/hadoop-yarn-site/YARN.html">YARN</A> (ou MRV2) est un gestionnaire de ressources. Son rôle est d’attribuer des ressources d'un cluster (CPU & mémoire) sous forme de conteneurs à une application demandeuse.
<br>*Note : une application demandeuse est un traitement qui s'exécute sur le cluster.*

### Les composants

Dans YARN, 2 composants entrent en jeu : le ResourceManager (RM) et le NodeManager (NM), ce couple de composants forme un système générique pour gérer les applications distribuées. 

#### ResourceManager
Ce composant gère l’ensemble des ressources du cluster, c’est lui qui a autorité pour attribuer les ressources aux applications demandeuses.
Il embarque un ordonnanceur qui priorise l’attribution des ressources aux différentes applications en accord avec certains paramètres définis au niveau du cluster (queue, limite, …).

#### NodeManager
Ce composant est présent sur chaque machine du cluster (comme le Datanode du HDFS), il surveille les ressources disponibles sur le nœud et remonte un état de ce dernier périodiquement au ResourceManager. Il est également en charge du lancement et de l’exécution des conteneurs. Il en existe deux types : ApplicationMaster et Container.

#### ApplicationMaster
Lorsque une application est lancée sur la cluster, le RessourceManager commence par demander l’instanciation d’un conteneur maître, l'Application Master qui va être en charge de : 
* réserver les ressources nécessaires à l’exécution de l’application auprès du ResourceManager
* suivre l’état de chaque conteneur de l’application
* gérer les échecs et relances de certains conteneurs
* fournir l’état global de l‘application au ResourceManager

#### Container
Il exécute une partie du traitement de l’application, il remonte son état auprès de son ApplicationMaster.

---
<!-- Slide 21 -->
<!--: .wrap -->
# YARN : interactions
![yarn](https://20100701.github.io/bigdata/static/images/yarn.png)

---
<!-- Slide 22 -->
<!--: .wrap -->
# Synthèse Hadoop
Ci-dessous un exemple de ce que pourrait être un cluster Hadoop minimal composé d'un Master et de trois Nodes.

![hadoop_synthese](https://20100701.github.io/bigdata/static/images/hadoop_synthese.png)

---
<!-- Slide 23 -->
<!--: .wrap bg=bg-white bg=aligncenter bgimage=https://images.unsplash.com/photo-1583791031153-d55e79f7f115?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1867&q=80 -->
# Thank you for your attention

