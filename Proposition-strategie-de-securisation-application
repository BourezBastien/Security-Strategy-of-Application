
# 🧐 Proposition de stratégie de sécurisation d'une application 

##  Introduction 

Hello, today we are going to talk about the security strategy. More specifically, we will discuss the risks and security issues to guarantee the integrity of the data that our future users will entrust to us through the application. 

## Sommaire 

- 🗺️ [La sécurisation d'une application]() 
	- 👀 [Que veut dire sécuriser une application ?]() 
- 🚨[Confidentialité]() 
- 📝 [Les stratégies générales de la sécurisation]() 
	- 🐱‍💻[Réduction de la surface d'attaque]() 
	- 🔒 [Moindre privilège]() 
	- ⛨ [Défense en profondeur]() 
- 💂 [Sécurisation Client]() 
	- [Inclusion de sécurité de contenus de tiers]()
		- Partage de ressources inter-origine (CORS)
		- Politique de sécurité du contenu (CSP)
		- Politique de la même origine (SOP)
		- Intégrité des sous-ressources (SRI)
	- [ClickJacking]()
	- [Requête silencieuse]()
	- [HTTPS / TLS / HSTS]()
	- [Politique de sécurité des mot de passe]()
- 💂 [Sécurisation Backend]() 
	- [Journalisation]()
	- [Sanitization]()
	- [Stratégie de sauvegarde]()
	- [Salage / Hashage / Sha256]()
	- [Authentification et Autorisation]()
	- [Strict mode]()
	- [Sessions]()
	- [RBAC]()
	- [Token (JWT)]()
- 💾 [Sécurisation BDD]() 
- 📡[Sécurisation API]() 

## 🔐 La sécurisation d'une application

Processus qui consiste à développer, ajouter et tester des fonctionnalités de sécurité au sein des **applications**, afin d'éviter l**es vulnérabilités** face à des menaces telles que **les accès et les modifications non autorisés**.


### Quoi ?

La gestion de la sécurité des applications est le processus qui consiste à développer, ajouter et tester des fonctionnalités de sécurité au sein des applications, afin d’éviter les vulnérabilités face à des menaces telles que les accès et les modifications non autorisés.

### Pourquoi ?

La sécurité des  **applications**  web est essentielle pour protéger les données, les clients et les organisations contre le vol de données, les interruptions de la continuité des activités ou d'autres conséquences néfastes de la cybercriminalité.

## ⚖️ Confidentialité

En sachant que votre application **vas être amener a recueillir des données utilisateur** ( nom, prénom, email, téléphone, pièces jointe ) il est **essentiel de noter** que ces **données** ne peuvent être **traitées ultérieurement** pour d’autres finalités, **surtout si elles sont incompatibles avec les finalités prévues initialement**.

> Si l’application propose des fonctionnalités permettant d’assurer un **service à distance** à son utilisateur et qu’elle comporte une connexion extérieure (ex : sauvegarde des données dans le  _cloud_), **des règles s’applique**.
> -   Les grands principes relatifs à la protection des données doivent être respectés, dès la conception de l’application («_Privacy by design »)_ ;
> -   Dans des hypothèses très précises, au regard de la finalité du traitement (ex : utilisation de l’application pour une recherche), des formalités doivent être réalisées ;
> -   Il est nécessaire de respecter toutes les obligations prévues par le règlement européen sur la protection des données (ex : réalisation d’une analyse d’impact, tenue du registre des activités de traitement, information des personnes, etc.).

> ⚠️ **Les données recueillies doivent être collectées pour des finalités déterminées, explicites et légitimes.** Elles ne peuvent être traitées ultérieurement pour d’autres finalités, surtout si elles sont incompatibles avec les finalités prévues initialement.

## 🤓 Les stratégies générales de la sécurisation
	
>![Image securité-ergonomie](https://i.imgur.com/fo8BBJr.png)
 La **stratégie de sécurisation d'une application** consiste à déterminer les sécurités qui vont être mises en place sur une application donner. Il est important de spécifier que si vous tirer plus vers la **sécurité** l'ergonomie de l'application sera impacté. **Cela est valable dans le sens contraire**.

### 🐱‍💻 Réduction de la surface d'attaque

![Image securité-ergonomie](https://i.imgur.com/O55lBp6.png)

Réduire votre **surface d’attaque** signifie mettre en place le plus de **protection en place** pour ainsi être moins **vulnérable à des attaques** ce qui laisse aux attaquants moins de moyens d’effectuer des attaques.
### Défense en profondeur


### 🔒 Moindre privilège

![Moindre privilèges](https://www.zscaler.fr/cdn-cgi/image/format%3Dauto/sites/default/files/images/page/xyz/zscaler-least-privilege-access-diagram-1.png)

Le **moindre privilèges** consiste a un système de **rôles hiérarchique**. Ces rôles on pour but de vérifier si la personnes a la permission d'accéder a une **ressource ou un services**.

### ⛨ Défense en profondeur

![Image de la défense en profondeur](https://www.riskinsight-wavestone.com/wp-content/uploads/2016/02/image1.png)

La défense en profondeur consiste à sécuriser son application **couche par couche** plutôt qu’à concentrer la protection à **un seul point de l’application**.

## 💂 Sécurisation Client


## Inclusion de sécurité de contenus de tiers


- CORS: **Permet à un site A d'autoriser le site B à lire des données (potentiellement privées) du site A (à l'aide du navigateur et des informations d'identification du visiteur, elle permet également de contourner le SOP)**


- SOP: **Partage des ressources entre différents sites Web,  mais empêche la lecture des informations de réponse HTTP**

- CSP: **Permet à un site de s'empêcher de charger du contenu (potentiellement malveillant) à partir de sources inattendues ou inconnus.**

- SRI: **Permet d’exposer, via l’attribut dédié integrity, le résultat attendu d’un hash réaliser sur un fichier ressources et le comparer au hash attendu et bloquer la ressource si les empreintes sont différentes.**

## 🍪 Cookie

![](https://oko.uk/wp-content/uploads/2019/12/cookie-types.jpg)

- Un **cookie** est un petit morceau de texte qui est **automatiquement enregistré** sur votre ordinateur par un **site** lorsque vous le parcourez.

Il permet au site de vous **reconnaître** et de conserver des **informations spécifiques à votre sujet**, comme vos données de connexion ou vos préférences linguistiques, et ce, afin que vous n’ayez pas à vous ré-enregistrer à chaque visite.

## 🖱️ ClickJacking

![](https://cdn.invicti.com/statics/img/ogimage/clickjacking-attacks.png)

 - Le **ClickJacking** (détournement de clic) est **une attaque qui amène un utilisateur à cliquer sur un élément de page Web qui est invisible ou déguisé en un autre élément** . Cela peut amener les utilisateurs à télécharger involontairement des logiciels malveillants, à visiter des pages Web malveillantes, à fournir des informations d'identification ou des informations sensibles, à transférer de l'argent ou à acheter des produits en ligne.
 
 ## 🔇 Requete silencieuse
 
![](https://s4.aconvert.com/convert/p3r68-cdx67/ah2o8-mac89.jpg)

 - Certaines fonctionnalités de la spécification HTML permettent de demander au navigateur d’émettre des requêtes silencieuses sans passer par l’exécution de code JavaScript ou CSS. Comme tout comportement qui conduit le navigateur d’une victime à initier une connexion de manière silencieuse, ces requêtes sont potentiellement indésirables et présentent des risques allant de la fuite d’informations jusqu’à l’exploitation de failles CSRF en passant par la réalisation d’attaques par déni de service distribué (DDoS).

## 📢 HTTPS / TLS / HSTS

![](https://cdn.searchenginejournal.com/wp-content/uploads/2021/08/what-is-https-6135eef3423dc-sej-1520x800.jpg)

- Le protocole de transfert hypertexte sécurisé (HTTPS) est la version sécurisée de [HTTP](https://www.cloudflare.com/learning/ddos/glossary/hypertext-transfer-protocol-http/) , qui est le principal protocole utilisé pour envoyer des données entre un navigateur Web et un site Web. HTTPS est crypté afin d'augmenter la sécurité du transfert de données. Ceci est particulièrement important lorsque les utilisateurs transmettent des données sensibles, par exemple en se connectant à un compte bancaire, à un service de messagerie ou à un fournisseur d'assurance maladie.

> HTTPS empêche les sites Web de diffuser leurs informations d'une manière facilement visible par toute personne fouinant sur le réseau.

###  TLS 

![](https://sectigostore.com/blog/wp-content/uploads/2020/05/tls-1-3-tls-version.jpg)

- **Transport Layer Security**, ou **TLS**, est un protocole de sécurité largement adopté conçu pour faciliter la confidentialité et la sécurité des données pour les communications sur Internet. Un cas d'utilisation principal de TLS est le chiffrement de la communication entre les applications Web et les serveurs, tels que les navigateurs Web qui chargent un site Web. TLS peut également être utilisé pour chiffrer d'autres communications telles que les e-mails, la messagerie et la voix sur IP (VoIP) .

> Le chiffrement TLS peut aider à protéger les applications Web contre les violations de données et autres attaques. Aujourd'hui, HTTPS protégé par TLS est une pratique standard pour les sites Web. Le navigateur Google Chrome a progressivement sévi contre les sites non HTTPS , et d'autres navigateurs ont emboîté le pas. Les internautes de tous les jours se méfient davantage des sites Web qui ne présentent pas l'icône de cadenas HTTPS.

###  HSTS

![](https://really-simple-ssl.com/wp-content/uploads/2022/09/Really-Simple-SSL-Visuals_Tekengebied-1-kopie.svg)

- Il est nécessaire de mettre en œuvre HSTS afin de limiter les risques d’attaque de type Man-In-The-Middle dus à des accès non sécurisés générés par les utilisateurs ou par un attaquant.

⚠️  **la pérennité de l’accès en HTTPS est un prérequis indispensable à HSTS, qui rendra l’accès en clair impossible.** 

Le mise en œuvre de HSTS se fait par la transmission d’un en-tête HTTP lors de l’accès au site en HTTPS pour assurer son intégrité. Par défaut, la stratégie HSTS d’un site est enregistrée par le navigateur lorsqu’il est visité pour la première fois (trust on first use). Pour combler cette vulnérabilité initiale, le gérant d’un site peut décider de l’inscrire à une « liste préchargée » (voir HSTS preload 10) de sites accessibles seulement en HTTPS, connue à l’avance par les navigateurs.

## 📋 Politique de sécurité des mot de passe

![](https://d1fmx1rbmqrxrr.cloudfront.net/zdnet/optim/i/edit/ne/2017/08/politique-mot-de-passe-620__w1200.jpg)

Il est recommandé de mettre en place une politique de sécurité des mots passe adaptée au contexte et aux objectifs de sécurité du système d’information.

- ⚠️ Pour cela il est recommander de suivre ce qui est dit par l'Anssi

	- **Imposer une longueur minimale pour les mots de passe**
	- **Ne pas imposer de longueur maximale pour les mots de passe**
	- **Mettre en œuvre des règles sur la complexité des mots de passe**
	- **Ne pas imposer par défaut de délai d'expiration sur les mots de passe des comptes non sensibles**
	- **Imposer un délai d'expiration sur les mots de passe des comptes à privilèges**
	- **Révoquer immédiatement les mots de passe en cas de compromission suspectée ou avérée**
	- **Mettre en place un contrôle de la robustesse des mots de passe lors de leur**
	- **Utiliser un sel aléatoire long**

## 💂 Sécurisation Backend

![Sécurisation backend illustrions](https://geekflare.com/wp-content/uploads/2021/09/Backend-solution.png)

## 📰 Journalisation

![](https://kinsta.com/fr/wp-content/uploads/sites/4/2022/08/journalisation-laravel.png)

Les journaux d’événements constituent une brique technique indispensable à la gestion de la sécurité des systèmes d’information. L’activité de journalisation est un moyen de détection des incidents de sécurité et d’analyse du comportement d’un site ou d’une application web. Cette activité concerne la phase de conception de l’application, pour la génération de journaux (ex. traçabiltié d’un changement de privilèges), ainsi que la phase d’exploitation de l’application, pour laquelle l’application des Recommandations de sécurité pour la mise en œuvre d’un système de journalisation est nécessaire. En effet, les recommandations portant sur l’horodatage des événements ainsi que sur la synchronisation des horloges entre les composants sont particulièrement pertinentes dans le cas d’une application web, bien souvent décomposée en plusieurs services amenés à générer leurs propres journaux de façon isolée.

## 🧹 Sanitization

![](https://s4.aconvert.com/convert/p3r68-cdx67/aaa57-0b0kd.png)


Cela signifie valider l'entrée avant de l'accepter à la fois sur le client et le serveur, et également filtrer, encoder ou autrement transformer une chaîne de texte afin qu'elle ne puisse pas être utilisée pour injecter du code en tant que JavaScript, SQL ou d'autres langages. En prévention de l'injection, outre la Sanitization, une option consiste à utiliser des versions paramétrées des API, comme l'envoi d'entrées en tant que paramètres de liaison aux instructions préparées à la base de données.

## 🗄️ Stratégie de sauvegarde

![](https://www.bemsp.fr/wp-content/uploads/2016/10/3-2-1-Datto.png)

Une stratégie de sauvegarde est un plan conçu pour garantir que les données essentielles de l'entreprise sont sauvegardées et prêtes à être restaurées en cas de perte de données. Les entreprises souffrent de tous les temps d'arrêt dûs à la perte de données, il est donc crucial de minimiser les temps d'arrêt autant que possible. La sauvegarde et reprise d’activité après incident sont essentielles pour garantir la continuité des opérations commerciales.

## Salage / Hashage / Sha256

![](https://connect.geant.org/wp-content/webp-express/webp-images/uploads/2022/01/EaPConnect-CyberSecurity-Workshop-II-990x556.jpg.webp)

🧂 Le salage de hachage de mot de passe se produit lorsque des données aléatoires - un sel - sont utilisées comme entrée supplémentaire dans une fonction de hachage qui hache un mot de passe. Le but du salage est **de se défendre contre les attaques par dictionnaire ou les attaques contre les mots de passe hachés**


🔪 Le  **hachage**, ou hashing en anglais, consiste littéralement à " hacher " des données, un message ou encore un texte afin de les réduire à une suite de caractères de courte longueur, appelée condensat. Pour cela, il faut utiliser un  **algorithme de hachage**.

Trois impératifs doivent être respectés :

-   La  **fonction de hachage**  doit être à sens unique ;
-   Il ne doit pas y avoir de collisions ; une fonction de hachage parfaite doit être en mesure d'éviter toute collision ;
-   La fonction de hachage doit être rapide pour être efficace ;
-   La moindre modification du contenu ou message d'origine doit entraîner une modification conséquente de la valeur de hachage.

**Sha256** est une fonction de **hachage** elle permet de ne pas stocker les mots de passe en clair dans la base de donnée  mais uniquement de stocker une empreinte de ces derniers. Il est important d’utiliser un algorithme public réputé fort afin de calculer les dites empreintes. **A ce jour, MD5 ne fait plus partie des algorithmes réputés forts**.


> De même, les fonctions de hachage publiques réputées fortes étant par nature à la disposition de tous, il est techniquement possible pour tout un chacun de calculer des empreintes. Aujourd’hui, on trouve facilement sur internet des dictionnaires immenses d’empreintes MD5 précalculées et, grâce à ces données, il est aisé de retrouver instantanément le mot de passe ayant été utilisé afin de générer ces empreintes. Afin de limiter ce risque, il est conseillé d’utiliser des fonctions spécialisées appelées « fonction de dérivation de clé », telles que PBKDF2 ou Argon2 par exemple, qui sont conçues spécifiquement pour stocker des mots de passe.


## 🎫 Authentification et Autorisation

![](https://www.okta.com/sites/default/files/styles/1640w_scaled/public/media/image/2020-10/Authentication_vs_Authorization.png?itok=uBFRCfww)

L’authentification est un mécanisme faisant intervenir deux entités distinctes : un prouveur et un vérifieur comme illustré par la figure 1.  

- Le prouveur cherche à prouver son identité au vérifieur. Il s’agit par exemple pour le prouveur de démontrer sa connaissance d’une donnée secrète comme un mot de passe. 
- Le vérifieur doit être capable de s’assurer de la validité de l’identité du prouveur. Il s’agit par exemple pour le vérifieur de contrôler l’exactitude du mot de passe fourni par le prouveur.

![Prouveur et vérifieur schéma](https://cdn.discordapp.com/attachments/440551059753140235/1037141818875314306/unknown.png)

Un prouveur est un utilisateur du système d’information cherchant à s’authentifier. Le vérifieur est quant à lui classiquement un serveur du système d’information qui a la charge de vérifier l’identité d’un utilisateur. 

Une étape préalable à l’authentification est l’étape de l’enregistrement. Cette étape consiste à enregistrer un prouveur (son identité, son moyen d’authentification, etc.) auprès d’un vérifieur. Cela correspond par exemple à la création d’un compte sur un site Web.

 L’authentification est précédée par une phase d’identification (parfois implicite) qui consiste, pour le prouveur, à annoncer son identité sans prouver cette dernière. Par exemple, il peut s’agir d’un nom d’utilisateur à renseigner.

**Résumer des différentes menace**

- **Recherche exhaustive**
	- Limite temporelle entre chaque essai (contre les attaquants en ligne) et fonctions de hachage itératives dédiées (contre les attaquants en ligne et hors ligne)
- **Recherche par dictionnaire**
	- Mots de passe robustes et aléatoires et coffrefort de mots de passe
- **Tables pré-calculées (rainbow table)**
	- Sel aléatoire long
- **Hameçonnage, ingénierie sociale**
	- Authentification multifacteur
## ⛔ Strict mode

![](https://nhidev.github.io/assets/img/strict-mode.jpg)

La syntaxe, pour déclarer le mode strict, a été conçue pour être compatible avec les anciennes versions de JavaScript.

Compiler un littéral numérique (4 + 5;) ou un littéral de chaîne ("John Doe";) dans un programme JavaScript n'a aucun effet secondaire. Il se compile simplement en une variable non existante et meurt.

Cela n'a donc `"use strict";`d'importance que pour les nouveaux compilateurs qui en "comprennent" le sens.

## Pourquoi le mode strict ?

Le mode strict facilite l'écriture de JavaScript "sécurisé".

Le mode strict transforme la "mauvaise syntaxe" précédemment acceptée en véritables erreurs.

Par exemple, en JavaScript normal, la saisie erronée d'un nom de variable crée une nouvelle variable globale. En mode strict, cela générera une erreur, rendant impossible la création accidentelle d'une variable globale.

En JavaScript normal, un développeur ne recevra aucun retour d'erreur en attribuant des valeurs aux propriétés non inscriptibles.

En mode strict, toute affectation à une propriété non inscriptible, une propriété getter uniquement, une propriété inexistante, une variable inexistante ou un objet inexistant génère une erreur.

## 🛅 Sessions

![](https://windowsreport.com/wp-content/uploads/2021/04/session-recording.jpg)

Une **session Web** est une série d'actions contiguës d'un visiteur sur un site Web individuel dans un laps de temps donné. Cela peut inclure vos recherches sur les moteurs de recherche, le remplissage d'un formulaire pour recevoir du contenu, le défilement d'une page de site Web, l'ajout d'articles à un panier, la recherche de billets d'avion ou les pages que vous avez consultées sur un seul site Web. Toute interaction que vous avez avec un seul site Web est enregistrée en tant que session Web sur la propriété de ce site Web.

>Pour éviter de stocker des quantités massives d'informations dans le navigateur, les développeurs utilisent des identifiants de session pour stocker les informations côté serveur tout en permettant la confidentialité des utilisateurs. Chaque fois qu'un utilisateur effectue une action ou fait une demande sur une application Web, l'application renvoie l'ID de session et l'ID de cookie au serveur, ainsi qu'une description de l'action elle-même.

⚠️ Il est recommandé qu’une session authentifiée ait une durée maximale de validité. Les secrets temporaires de sessions (comme des cookies par exemple) doivent avoir une durée de vie limitée. Il est ainsi recommandé de forcer la ré-authentification des utilisateurs après une période adaptée au cas d’usage.

## 🔏 RBAC

![](https://assets-global.website-files.com/622642781cd7e96ac1f66807/62d0f09bf0c56e7859434cb7_052021-Harness-Blogpost-CD-ShareCard-RBAC.png)

Le contrôle d'accès basé sur les rôles (RBAC), également connu sous le nom de sécurité basée sur les rôles, est un mécanisme qui restreint l'accès au système. Cela implique de définir des autorisations et des privilèges pour permettre l'accès aux utilisateurs autorisés. La plupart des grandes entreprises utilisent le contrôle d'accès basé sur les rôles pour fournir à leurs employés différents niveaux d'accès en fonction de leurs rôles et responsabilités. Cela protège [les données sensibles](https://www.imperva.com/learn/data-security/sensitive-data/) et garantit que les employés peuvent uniquement accéder aux informations et effectuer les actions dont ils ont besoin pour faire leur travail.

## 🗝️ Token (JWT)

![](https://www.cronj.com/blog/wp-content/uploads/JWT-1.png)

JSON Web Token (JWT) est une norme ouverte ( [RFC 7519](https://tools.ietf.org/html/rfc7519) ) qui définit un moyen compact et autonome pour transmettre en toute sécurité des informations entre les parties en tant qu'objet JSON. Ces informations peuvent être vérifiées et approuvées car elles sont signées numériquement. Les JWT peuvent être signés à l'aide d'un secret (avec l' algorithme **HMAC** ) ou d'une paire de clés publique/privée utilisant **RSA** ou **ECDSA** .

Bien que les JWT puissent être chiffrés pour assurer également le secret entre les parties, nous nous concentrerons sur les jetons _signés ._ Les jetons signés peuvent vérifier l' _intégrité_ des revendications qu'ils contiennent, tandis que les jetons chiffrés _cachent_ ces revendications aux autres parties. Lorsque les jetons sont signés à l'aide de paires de clés publique/privée, la signature certifie également que seule la partie détenant la clé privée est celle qui l'a signée.

### Avantages de l'utilisation de jetons

-  **L'authentification basée sur les jetons est plus évolutive et efficace**

	- Comme nous savons que les jetons doivent être stockés du côté de l'utilisateur, ils offrent une solution 			évolutive.

	- De plus, le serveur a juste besoin de créer et de vérifier les jetons avec les informations, ce qui signifie qu'il est possible de maintenir plus d'utilisateurs sur un site Web ou une application à la fois sans aucun problème.
	
- **Flexibilité et performances**

	- La flexibilité et les performances globales améliorées sont d'autres aspects importants en ce qui concerne l'authentification basée sur les jetons, car ils peuvent être utilisés sur plusieurs serveurs et ils peuvent offrir une authentification pour divers sites Web et applications à la fois.

	- Cela contribue à encourager davantage d'opportunités de collaboration entre les entreprises et les plates-formes pour une expérience sans faille.
	
- **Les jetons offrent une sécurité robuste**

	- Étant donné que les jetons comme JWT sont sans état, seule une clé secrète peut la valider lorsqu'elle est reçue dans une application côté serveur, qui a été utilisée pour la créer.

	- Par conséquent, ils sont considérés comme le moyen le meilleur et le plus sûr d'offrir une authentification.

### Inconvénients de l'utilisation de jetons

- **Clé secrète compromise**

	- L'un des principaux inconvénients de s'appuyer sur des jetons est qu'il ne repose que sur une seule clé. Oui, JWT n'utilise qu'une seule clé, ce qui, s'il est mal géré par un développeur/administrateur, entraînerait de graves conséquences pouvant compromettre des informations sensibles.

	- Il est essentiel pour les entreprises de rechercher une aide professionnelle associée à des mécanismes de sécurité robustes tout en prévoyant d'ajouter JWT à leur mécanisme d'authentification pour garantir le plus haut niveau de sécurité.
	
-  **Surcharge de données**

	- La taille globale d'un JWT est bien supérieure à celle d'un jeton de session normal, ce qui le rend plus long chaque fois que plus de données y sont ajoutées.

	- Ainsi, si vous ajoutez plus d'informations dans le jeton, cela aura un impact sur la vitesse de chargement globale et entravera ainsi l'expérience utilisateur.

	- Cette situation peut être corrigée si les bonnes pratiques de développement sont suivies et que des données minimales mais essentielles sont ajoutées au JWT.

-  **Durée de vie plus courte**

	- Les JWT de courte durée sont plus difficiles à utiliser pour les utilisateurs. Ces jetons nécessitent une réautorisation fréquente, ce qui peut parfois être ennuyeux, en particulier pour les clients.

	- L'ajout de jetons d'actualisation et leur stockage approprié est le seul moyen de résoudre ce scénario dans lequel des jetons d'actualisation à longue durée de vie peuvent aider les utilisateurs à rester autorisés pendant une période plus longue.

## 💾 Sécurisation BDD
## 📡 Sécurisation API
