# Stratégie de sécurisation d'une application
  
  ## Introduction

![Image securité-ergonomie](https://i.imgur.com/fo8BBJr.png)

> La **stratégie de sécurisation d'une application** consiste à déterminer les sécurités qui vont être mises en place sur une application donner. Il est important de spécifier que vous si vous tirer plus vers la **sécurité** l'ergonomie de l'application sera impacté cela est **valable dans le sens contraire**.

</br>

## Sommaire

- [Réduction de la surface d'attaque]()
- [Défense en profondeur]()
- [Moindre privilèges]()

- FontEnd

	-  [Sécurités modernes côté client]()
		-  Partage de ressources inter-origine (CORS)
		-  Politique de sécurité du contenu (CSP)
		-  Politique de la même origine (SOP)
		-  Intégrité des sous-ressources (SRI)
	-  [Cookie]()
	-  [ClickJacking]()
	-  [Requete silencieuse]()
	-  [HTTPS / TLS / HSTS]()
	-  [Politique de sécuriter des mot de passe]()
- BackEnd
	-  [API stateless]()
	-  [List item]()
	-  [Sha256]()
	-  [Journalisation]()
	-  [Sanitization]()
	-  [Stratégie de sauvegarde]()
	-  [Salage]()
	-  [Hashage]()
	-  [Authentification et Autorisation]()
	-  [Strict mode]()
	-  [Sessions]()
	-  [RBAC]()
	-  [Token]()
	-  [Sécurisation d'authetification]()
	-  [Sécurisation d'API]()
- Faille de sécuriter
	-  [Compromission des ressources applicatives]()
	-  [Point d'eau]()
	-  [DDOS]()
	-  [le vol de donée]()
	-  [XSS]()
	-  [CSRF]()
	-  [SQLI]()
- Prestataires
	-  [BugBounty]()
	-  [Audit]()


</br>
</br>

### Réduction de la surface d'attaque

![Image securité-ergonomie](https://i.imgur.com/O55lBp6.png)

Réduire votre **surface d’attaque** signifie mettre en place le plus de **protection en place** pour ainsi être moins **vulnérable à des attaques** ce qui laisse aux attaquants moins de moyens d’effectuer des attaques.

### Défense en profondeur
![Data center](http://www.france-datacenter.fr/wp-content/uploads/2015/01/Datacenter-Google.jpg)
La défense en profondeur consiste à sécuriser son application **couche par couche** plutôt qu'à concentrer la protection à **un seul point de l'application**.

> **Exemple**: pour cet exemple nous allons prendre un datacenter, les datacenters sont conçus sous forme de niveaux et chaque niveau possède ses propres sécurisés en plus de celle déjà mis en place au niveau précèdent.

### Moindre privilèges

![Moindre privilèges](https://www.zscaler.fr/cdn-cgi/image/format%3Dauto/sites/default/files/images/page/xyz/zscaler-least-privilege-access-diagram-1.png)

Le **moindre privilèges** consiste a un système de **rôles hiérarchique**. Ces rôles on pour but de vérifier si la personnes a la permission d'accéder a une **ressource ou un services**.

> **Exemple**:  Au dessus nous avons dit qu'un datacenter était constitué sous forme de niveaux pour chaque niveaux nous allons appliquer le **moindre privilège** pour faire en sorte que seules des personnes habiliter on accède aux serveurs, ce système est également mis aux niveaux inférieurs.

**Pourquoi ?**

-   **Il réduit la surface exposée aux cyberattaques.**  Aujourd’hui, la plupart des attaques s’appuient sur  l’exploitation des identifiants à privilèges. En limitant les privilèges l’application du moindre privilège permet de réduire la surface d’attaque globale.
-   **Il stoppe la propagation de logiciels malveillants (malware).** Les attaques de logiciels malveillants sont incapables d’utiliser des privilèges élevés pour accroître leur accès afin de se déplacer latéralement pour installer ou exécuter des programmes ou endommager la machine.
-   **Il améliore la productivité des utilisateurs.**  La suppression de droits d’administrateur permet de réduire le risque, tandis que la mise en place de l’élévation de privilèges « juste à temps », basée sur une politique, préserve la productivité des utilisateurs en évitant de trop solliciter l’assistance informatique.
-   **Il rationalise la conformité et les audits.**  De nombreuses politiques internes et exigences réglementaires requièrent que les organisations implémentent le principe du moindre privilège sur les comptes à privilèges afin d’éviter toute dégradation des systèmes critiques, intentionnelle ou non. L’application du moindre privilège aide les organisations à prouver leur conformité en fournissant un journal d’audit complet des activités à privilèges.

## FontEnd

### Sécurités modernes côté client

La **Sécurités modernes côté client** consiste a un ensemble de termes (CORS, SOP, CSP, SRI). Le **Partage de ressources inter-origine (CORS)** permet à un site A d'autoriser le site B à lire des données (potentiellement privées) du site A (à l'aide du navigateur et des informations d'identification du visiteur). La **Politique de la même origine (SOP)** partage des ressources entre différents sites Web, mais empêche la lecture des informations de réponse HTTP. **La Politique de sécurité du contenu CSP** permet à un site de s'empêcher de charger du contenu (potentiellement malveillant) à partir de sources inattendues ou inconnus. **Intégrité des sous-ressources (SRI)** permet d’exposer, via l’attribut dédié **integrity**, le résultat attendu d’un **hash** réaliser sur un fichier ressources et le comparer au has attendu et bloquer la ressource si les empreintes sont différentes.

**Pourquoi ?**

 > Cet **ensemble de termes** on voyait le jour afin de réduire la **surface d'attaque d'un site / application web**. Il offre également la **possibilité de partager du contenu** à travers plusieurs sites.

### Cookie

Un cookie est un *élément de données d'un site Web** qui est stocké dans un **navigateur Web** et que le site Web peut **récupérer ultérieurement**.
