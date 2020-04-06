### Jour 4 / 5

# Semaine d'introduction au code

## Réalise le site de présentation de ta startup ou de ton association étudiante !

# Cours : Atomic Design

## 1\. Introduction

Quand tu vas sur un site, as-tu déjà remarqué que beaucoup d'éléments reviennent souvent ? Les [formulaires](http://bootstraplovers.com/assan-kit-3.8/bootstrap4/admin-dashboardUi/html/form-elements.html), par exemple. Ou encore, ces [petits badges](https://uxpowered.com/products/appwork/v120/html-demo/ui_badges.html) qui t'indiquent combien de notifications tu as.

Bienvenue dans l'univers magique du composant web ! Tous les sites utilisent vraiment les mêmes... Le point fort de cette technique, c'est qu'il suffit d'en gérer une vingtaine pour peupler une grande partie du site. Ils t'aident aussi à créer des sections facilement, comme le montre ce dessin de [Audrey Hack](https://medium.com/scribe/comment-concevoir-un-syst%C3%A8me-de-composants-en-atomic-design-770b910f4f32) :

![](https://i.imgur.com/J5WHIMK.jpg)  

Pour passer des composants à des sections plus complexes, je t'invite à jeter un oeil à [cette vidéo](https://www.youtube.com/watch?v=8EuZD6Hsbxk) de Bitovi, puis à [ce super article](https://medium.com/@audreyhacq/l-atomic-design-une-m%C3%A9thode-de-co-creation-prometteuse-bd9d5fc2b2ad) d’Audrey Hacq sur le principe de l'Atomic Design.

En gros, il existe plein de composants basiques (boutons, formulaires, etc) qui peuvent s'ajouter pour former des sections de pages (formulaire d'inscription, header, etc). Ces mêmes sections se superposent ensuite pour former une page internet.

## 2\. Contexte et historique

En 2016, un certain Brad Frost sort un livre où il reconsidère la façon dont les pages web sont conçues : [Atomic Design](http://atomicdesign.bradfrost.com/). Cette théorie propose de voir les pages web non pas comme celles d'un livre, mais comme une construction de briques basiques à réutiliser dans l'application entière. Dans ses conférences, il aime citer Stephen Hay pour expliciter sa théorie :

> We're not designing pages, we're designing systems of components
> 
> **Stephen Hay**

Avec l'avènement de Bootstrap, le design par composants s'est vraiment popularisé. Boutons, formulaires, cartes et autres navbars se retrouvent maintenant dans une majeure partie du web, devenant les seuls éléments différenciants d'une application. Afin d'éviter que tous les sites ne ressemblent à des clones de Bootstrap, les designers ont commencé à sortir des kit UI (sorte de charte graphique appliquée aux éléments de ta page).

Prends donc le temps de visionner cette [super conférence](https://www.youtube.com/watch?v=CBsWl5uCaEs) d'Audrey Hacq pour comprendre, en 30 minutes, les enjeux et la raison d'être de l'Atomic Design.

## 3\. La ressource

### 3.1\. Le principe de l'Atomic Design

Quand on fait de l'Atomic Design, on va de l'atome à la page :

![](https://i.imgur.com/0WvV2F2.png)  

#### 3.1.1\. Les atomes

Les atomes sont les composants de base. Il peut s'agir d'un bouton, d'un icône, ou d'un champ de formulaire. Tu peux en trouver une liste sur [le site de Bootstrap](https://getbootstrap.com/docs/4.1/components/alerts/). Par exemple, voici un bouton :

![signup button](https://i.imgur.com/NGw4ouy.png)

#### 3.1.2\. Les molécules

Les molécules sont des assemblages d’atomes (composants) qui forment des composants d’interface simples. Cela peut être une "price card", un formulaire, ou encore une navbar. Voici un exemple de molécule faite avec l'atome ci-haut :

![pricing](https://i.imgur.com/Vl8iZmy.png)

#### 3.1.3\. Les organismes

Les organismes sont des assemblages de molécules formant une partie de la page finale de ton site. Il peut s'agir d'un formulaire d'inscription, d'une section "produits suggérés", ou encore d'une sidebar. Voici un exemple d'organisme réalisé avec la molécule précédente :

![pricing](https://i.imgur.com/7JWk7QC.png)

#### 3.1.4\. Les templates

C'est la page finale. Par exemple la page d'inscription, ou bien la page pricing. [Voici un exemple](https://getbootstrap.com/docs/4.1/examples/pricing/) de page template, fait avec l'organisme vu plus haut.

### 3.2\. Atomic Design et Bootstrap

#### 3.2.1\. Penser composants

Comme tu l'a compris, l'Atomic Design permet de décomposer rapidement une page web. Résultat : au lieu d'un rendu style "livre moche des années 90", tu te retrouves avec une page qui a vraiment de la gueule grâce à un assemblage d'éléments qui claquent.

Comme tout framework, Bootstrap possède l'intégralité des composants classiques [que tu peux retrouver ici](https://getbootstrap.com/docs/4.3/components/). Tu peux jeter un œil sur leurs exemples de [cards](https://getbootstrap.com/docs/4.3/components/card/), ou ceux de [navbars](https://getbootstrap.com/docs/4.3/components/navbar/). Ces composants forment la base du design web classique. À partir de maintenant, tu devras réfléchir avec eux.

Pour obtenir plein d'exemples de molécules et d'organismes, regarde [la page d'exemples](https://getbootstrap.com/docs/4.3/examples/) de Bootstrap ou encore [la page de templates](https://www.w3schools.com/bootstrap/bootstrap_templates.asp) de W3Schools. Je te conseille quand même de ne pas te prendre la tête pour tes projets THP codés sur 1 demi-journée, et de réutiliser ces super exemples pour tes pages. Tu parviendras à créer des sites qui en jettent, avec de bonnes structures, en quelques copier-coller à peine. Tes correcteurs apprécieront !

Depuis que j'utilise Bootstrap, je n'ai plus de fichier `style.css`. Plus besoin de modifier les composants ou de faire de la mise en page ! Bootstrap s'occupe de tout. Si j'ai envie de faire un truc précis, je m'arrange pour m'adapter au composant actuel. En plus d'ajouter de la cohérence à mon site internet, ça m'évite de faire du CSS tout moche et de devoir réinventer la roue en design. **Nous allons donc te demander de faire de même jusqu'à la fin de la semaine de HTML/CSS**.

#### 3.2.2\. Des surcouches de Bootstrap pour changer ton design

Le design de base de Bootstrap de base est suffisant pour faire des applications basiques mais il reste, avouons-le, assez limité. De plus, il y a plein d'organismes difficiles à réaliser sans toucher au CSS. Pour pallier à ce double problème, nous allons te donner des ressources pour ajouter un joli coup de boost à tes applications Bootstrap.

Prenons l'exemple du Hero que tu as du refaire hier à la main. Ce serait bien d'avoir un thème qui l'inclut directement, n'est-ce pas ? Oeuvrer pour moins de prise de tête, c'est toujours une bonne idée.

##### 3.2.2.1\. Petite surcouche simple d'utilisation

Il existe un site appelé [Bootswatch](https://bootswatch.com/) proposant une multitude de légères modifications à Bootstrap, super faciles à installer. Le principe de grille, composants, div reste le même. Seules changent les couleurs, polices et formes des composants pour que ton site soit un peu moins "standardisé".Va donc jeter un oeil [sur les différents "thèmes" qu'ils proposent](https://bootswatch.com/) ! Perso j'aime bien [Flatly](https://bootswatch.com/flatly/).

Petit entraînement : installe ce thème sur ta page de pricing.

##### 3.2.2.2\. Vrais thèmes de pros

Bootstrap est excellent pour les atomes et la mise en page. Par contre, au niveau des molécules et organismes, il en manque quand même quelques-uns (la page d'exemples est un peu limitée). Je pense par exemple à une sidebar pour un dashboard, ou alors une fiche produit simple. Le principe du design atomique est d'avoir plein de molécules et organismes qu'il suffit de réutiliser dans le bon contexte, donc ce serait cool d'avoir davantage d'exemples de pages toutes faites...

Pour ça, il existe des thèmes ([Bootstrap fait payer les siens](https://themes.getbootstrap.com/)) que tu peux ajouter à ton projet : il s'agit d'un ensemble de fichiers CSS fournissant plein d'organismes et pages d'exemples pour t'amuser. Par exemple, tu peux avoir un organisme de [témoignages](http://themes.getbootstrap.com/preview/?theme_id=4231&show_new=) ou bien un organisme d'[état d'un projet](https://keenthemes.com/keen/preview/demo2/). L'autre avantage des thèmes, c'est qu'ils vont généralement modifier le design de base des composants Bootstrap : parfait pour faire un site original !

Voici deux sites sympa pour gratter des thèmes gratuits : [StartBootstrap](https://startbootstrap.com/) en recense quelques uns pas trop moches, par exemple [un dashboard admin simple](https://blackrockdigital.github.io/startbootstrap-sb-admin/), ou bien [un petit one-pager efficace](https://blackrockdigital.github.io/startbootstrap-grayscale/). Dans le même genre, [TemplateMag](https://templatemag.com/bootstrap-templates/) est pas mal non plus.

Cependant, si l'univers du code est en général très open source, il est difficile de trouver des thèmes et template de front gratuits. Déjà, en matière de design, y a pas photo : tu peux comparer la qualité des formulaires entre [ce thème](https://templatemag.com/demo/templates/Dashio/form_component.html) (gratuit) et [celui-ci](https://keenthemes.com/keen/preview/demo2/components/forms/controls/base.html) (payant). Je précise que j'ai choisi, pour le gratuit, le plus populaire (et de loin) sur TemplateMag. Enfin, en termes d'organismes, un thème payant aura 100 fois plus de pages exemples qu'un thème gratuit (souvent one-pager). Encore une fois, tu peux facilement constater la différence entre [ce thème](https://blackrockdigital.github.io/startbootstrap-creative/) (gratuit) et [celui-là](http://themes.getbootstrap.com/preview/?theme_id=5348&show_new=) (payant). Quitte à installer un thème pour avoir plus de pages exemples et un design plus chiadé, autant ne pas le faire à moitié et mettre la main au portefeuille.

Si tu es prêt à payer, je te conseille 2 options : celui de Bootstrap propose [des thèmes](https://themes.getbootstrap.com/) à la fois jolis, complets et évidemment compatibles avec le reste des éléments du site. Le site [WrapBootstrap](https://wrapbootstrap.com/) propose aussi pas mal de thèmes Bootstrap pas trop chers et complets.

>#### 🚀 ALERTE BONNE ASTUCE
>
>Si THP n'a pas le droit d'acheter des thèmes Bootstrap et de vous les filer, nous ne pouvons pas empêcher une bande d'une cinquantaine de moussaillons d'acheter un thème à 50 $ et de se le partager via WeTransfer ou autre.
>
>Pour le moment vous n’en avez pas besoin, mais dans le futur... très sûrement 😎.


## 4\. Pour aller plus loin

Voici quelques ressources pour mieux appréhender le design atomique :

*   La [conférence de Brad Frost](https://www.youtube.com/watch?v=VVUpVVWZULw) sur le sujet est la référence en la matière.
*   Nous conseillons les écrits d'Audrey Hacq, dans l'ordre :
    1.  [L’atomic design, une méthode de co-création prometteuse](https://medium.com/@audreyhacq/l-atomic-design-une-m%C3%A9thode-de-co-creation-prometteuse-bd9d5fc2b2ad).
    2.  [Tout savoir sur les Systèmes de Design](https://medium.com/@audreyhacq/tout-savoir-sur-les-syst%C3%A8mes-de-design-1b6400c9a1b3).
    3.  [L’atomic design et la créativité](https://medium.com/@audreyhacq/latomic-design-et-la-cr%C3%A9ativit%C3%A9-b17fd332829c).
    4.  [Comment concevoir un système de composants en atomic design ?](https://medium.com/scribe/comment-concevoir-un-syst%C3%A8me-de-composants-en-atomic-design-770b910f4f32)

# Cours : Marketing web : comment construire un site qui sert à quelque chose

## 1\. Introduction

Pour éviter de finir avec un site incompréhensible, laid et ennuyeux au possible, il est important de savoir se poser et se demander quoi coder. Avant de foncer tête baissée, prends donc le temps de te mettre dans la peau d'un futur utilisateur et de te poser les bonnes questions :

1.  Pourquoi est-il venu sur ton site ?
2.  Comment lui faire comprendre le plus simplement possible ce que fait ton site ?
3.  Qu'ai-je envie de lui faire faire ?
4.  Ai-je passé assez de temps à designer un truc qui donne envie ?

Je vois énormément de moussaillons qui foncent la fleur au fusil et codent le site de leur association ou de leur _startup nation_ sans se poser ces questions. Résultat: des sites moches ET incompréhensibles. Les 2 heures gagnées en évitant une vraie réflexion préliminaire seront finalement perdues dans des campagnes marketing qui feront fuir les utilisateurs. Permettez-moi de me citer encore une fois :

> Le code est un outil : si l'on s'en sert bien, il peut faire de belles choses. Si l'on s'en sert mal, ce marteau produira des clous tordus.
> 
>**Moi-même, personne absolument pas mégalo**

En t'encourageant à te poser les trois premières questions vues ci-haut, cette ressource te fourniras quelques tips en marketing adaptés aux pages d'accueil de sites internet.

## 2\. Contexte et historique

Avec l'avènement d'Internet, le design de pages web est une science très étudiée, et qui répond à des codes bien précis. L'un des grand précurseurs de la discipline est [Paul Graham](https://fr.wikipedia.org/wiki/Paul_Graham), ingénieur de formation et fondateur de Y Combinator, l'incubateur le plus prestigieux sur Terre .

Créée en France en 2013, The Family a fortement popularisé le sujet dans les cercles des startup-parisiens en reprenant plus ou moins les écrits de Paul Graham dans des conférences.

## 3\. La ressource

### 3.1\. Les bases

Let's _start with why_ ! L'une des choses les plus importantes à faire en marketing est de se demander pourquoi toi, tu existes. Qu'est-ce qui te définit. Comme dirait Simon Sinek dans [sa très célèbre conférence](https://www.ted.com/talks/simon_sinek_how_great_leaders_inspire_action) :

> People don't buy what you do; they buy why you do it. And what you do simply proves what you believe
> 
> **Simon Sinek**

Si tu ne l'as pas fait, nous t'invitons à regarder cette conférence, l'une des plus célèbres de TED.

Pour en savoir plus sur l'art entourant les pages d'accueil de sites, nous allons te présenter une conférence de The Family. On aime ou on n'aime pas l'organisation, mais on ne peut nier que leur impact dans l'univers web/produit a été significatif à l'époque de leur lancement (2013-2014). Ils ont vraiment posé les jalons de ce qui allait devenir LE site web moderne en France.

La vidéo est celle d'Oussama Ammar sur [les erreurs à ne pas faire sur votre homepage](https://www.youtube.com/watch?v=ixa_fiF1Dqs). En trente minutes, il explique les notions de proposition de valeur, les boutons de partage, et _call to action_. Il termine en disant que "si la plupart des gros sites mondiaux ont une optique de _tu t'inscris ou tu dégages_, cette stratégie peut ne pas convenir à tout le monde : réfléchissez bien à ce que vous voulez obtenir dans la conversion de votre visiteur", ce qui est une fantastique leçon d'humilité.

### 3.2\. Les éléments que l'on retrouve dans la page

Pour cette partie, tout dépend de ce que tu veux faire et promouvoir. La page d'accueil d'un restaurant sera différente de celle d'une association étudiante. Voici néanmoins ce que tu risques de voir très souvent :

*   Le Hero, avec la proposition de valeur et très souvent le _call to action_.
*   Le _call to action_ (invitation à Liker la page Facebook, inscription à une newsletter, etc).
*   Une présentation du produit.

## 4\. Points importants à retenir

Avant de foncer tête baissée dans du code, pense et modélise la page que tu souhaites faire.

## 5\. Pour aller plus loin

Y'a à boire et à manger sur le sujet, mais [la chaîne Youtube de The Family](https://www.youtube.com/channel/UCYxgidQYV3WPD0eeVGOgibg) propose quelques vidéos super bien pour le marketing web.

# Cours : Ce que le web nous propose : quels outils nous recommandons pour gagner du temps de productivité

## 1\. Introduction

Il existe sur le web une multitude d'outils super pratiques qui te feront gagner un temps fou ! J'en ai quelques uns à te conseiller aujourd'hui, triés par catégorie :

*   **Les outils de travail** : ils servent à remplacer l'utilisation non pertinente de Microsoft Word (Word pour une liste _to-do_, c'est NON) et à centraliser l'information de travail importante.
*   **Les outils d'automatisation** : plutôt que de coder ou faire soi-même des trucs répétitifs, l'utilisation de ce genre d'outils te fera gagner un temps précieux.
*   **Les outils qui font des sites à ta place** : apprendre à coder, c'est bien. Savoir à quel moment il est pertinent d'utiliser tes compétences en code plutôt que passer par un service proposant de faire des landing pages à ta place, c'est encore mieux.
*   **Les extensions inspirantes** : nous t'en listerons quelques unes qui rendront tes ouvertures de nouvel onglet plus agréables.

Pour ces services, nous avons retenus comme facteurs importants : le design, le prix extrêmement accessible (la totalité des services proposés ont une version gratuite), la praticité, et le temps gagné. Nous avons donc écarté certains outils potentiellement supérieurs sur d'autres points (exhaustivité des fonctionnalités, open source, etc) mais moins intéressants par rapport à nos critères.

## 2\. La ressource

### 2.1\. Les outils de travail

#### 2.1.1\. Trello

[Trello](https://trello.com/) est un outil de gestion de projets à la fois léger, customisable, et proposant une version gratuite très permissive. On peut s'en servir pour tout : [une liste de courses pour les colocs](https://trello.com/b/Wl8XMqMZ/liste-de-courses-colocation), [la planification d'un anniversaire surprise d'un ami](https://trello.com/b/aIYRYpzd/anniversaire-surprise-de-benjamin-30-ans), [ta recherche d'emploi](https://trello.com/b/lFYXqEck/comment-trouver-job-de-vos-r%C3%AAves)...

Perso, j'ai quelques tableaux Trello où je note mes tâches personnelles. Je trouve ça tellement pratique que je ne peux que t'encourager à tester ! [Voici un guide](https://trello.com/guide) pour apprendre à t'en servir.

#### 2.1.2\. La suite Google

Ok, celui-là peut paraitre un peu évident, mais il reste assez sous-estimé. La [suite Google](https://www.google.com/drive/) est une tuerie permettant de faire énormément de choses ! Déjà, ils proposent gratuitement la suite Office (avec moins de fonctionnalités, certes. Mais rien de vraiment bloquant). Cerise sur le gâteau : ils ont aussi la meilleure solution de collaboration de fichiers _office_ du marché !

Et c'est pas fini. Ils ont d'autres avantages :

*   Automatisation facile : avec eux, coder un programme automatisant un fichier Google Spreadsheet devient presque aussi facile qu'un branchement Zapier.
*   Compatibilité universelle : ils rendent le partage de fichiers vraiment simple, puisqu'un navigateur internet permet de le faire. Pas de problème de compatibilité `.doc` ou `.odt` qui ne servent à rien.
*   Ils proposent une foultitude de templates faciles à utiliser (prends ça, Word et tes templates inutilisables !).

#### 2.1.3\. Notion

Nouveau chouchou de la startup nation, [Notion](https://www.notion.so/) est une sorte de version stylée de Trello et la suite Google réunis.

### 2.2\. Les outils d'automatisation

Faire des tâches répétitives à la main, c'est long. Nous allons donc t'indiquer des outils pour les automatiser et te faire gagner du temps.

### 2.2.1\. Zapier

[Zapier](https://zapier.com/), c'est vraiment de la bombe. Cet outil sert à automatiser les liens entre deux applications connues. Par exemple : si un utilisateur remplit un formulaire sur Google Forms, ça va créer une carte sur Trello. Ou encore : si tu reçois un email de ta grand-mère, un SMS va t'en avertir. Les possibilités sont infinies ! Grâce à Zapier, tu peux automatiser un grand nombre de tes tâches quotidiennes. C'est en quelque sorte une version qui est bien de [IFTTT](https://ifttt.com/) (pour ceux qui connaissent).

### 2.2.2\. Mailchimp

[Mailchimp](https://mailchimp.com/) est un service de gestion d'emails, où tu peux inscrire des utilisateurs à une mailing list, designer des campagnes d'email, les envoyer, puis analyser les résultats (taux d'ouverture, taux de clics, etc).

C'est très pratique pour envoyer des newsletters, et/ou gérer les abonnés à tes emails.

### 2.2.3\. Un gestionnaire de mots de passe

Difficile de se passer d'un gestionnaire de mots de passe, de nos jours. Ce type de service propose de stocker tous tes mots de passe de manière sécurisée, afin de pouvoir en utiliser des plus complexes pour chaque site que tu utilises (finis les ["password1234"](https://www.journaldugeek.com/2017/12/20/voici-la-liste-des-25-mots-de-passe-les-plus-populaires-et-probablement-les-moins-surs-de-2017/) et autres carnets papiers oubliés dans le bus avec tous tes codes !).

Sachant que 1\. la majorité des gens utilisent le même mot de passe partout, et que 2\. certains sites se font pirater leur base de données, la plupart des adresses emails ont au moins un mot de passe qui a déjà été piraté (comme tu peux le constater [sur ce site)](https://haveibeenpwned.com/Passwords). Oups ?

C'est pourquoi nous te recommandons d'utiliser un gestionnaire de mots de passe pour éviter de futurs désagréments. Voici mes préférés :

*   [LastPass](https://www.lastpass.com/fr)
*   [BitWarden](https://bitwarden.com/)
*   [1Password](https://1password.com/fr/)

### 2.3\. Les outils qui font des sites à votre place

C'est cool d'apprendre les bases du code pour comprendre comment ça marche. Mais savais-tu qu'il existait des solutions pour faire de belles pages à ta place ? Des fois, ça a du bon d'être un peu flemmard 😸

#### 2.3.1\. Wordpress

Très connu, [Wordpress](https://fr.wordpress.org/) est une solution puissante qui génère et gère des sites. Son côté usine à gaz peut en rebuter plus d'un, mais si tu veux faire un blog sans faire trois mois de code, c'est une bonne alternative.

#### 2.3.2\. Squarespace

Tu veux un site vitrine cool pour ton entreprise ? Une boutique en ligne sans faire trois mois de code ? [Squarespace](https://fr.squarespace.com/) est là pour toi. Il s'agit d'une plateforme aidant les professionnels à lancer rapidement un site répondant à un besoin partagé par d'autres professionnels (boutique en ligne, page pour un restaurant, portfolio pour un photographe, etc).

#### 2.3.3\. Landen

[Landen](https://www.landen.co/) permet de générer facilement de jolies landing pages.

Dans le même genre, nous recommandons aussi [Strikingly](https://www.strikingly.com/).

## 3\. Points importants à retenir

Nous t'avons donné quelques outils pour mieux travailler, dont voici un récapitulatif :

*   Les outils de travail
    *   [Trello](https://trello.com/)
    *   [La suite Google](https://www.google.com/drive/)
    *   [Notion](https://www.notion.so/)
*   Les outils d'automatisation
    *   [Zapier](https://zapier.com/)
    *   [Mailchimp](https://mailchimp.com/)
    *   Un gestionnaire de mots de passe
*   Les outils qui font des sites à votre place
    *   [Wordpress](https://fr.wordpress.org/)
    *   [Squarespace](https://fr.squarespace.com/)
    *   [Landen](https://www.landen.co/)
    *   [Strikingly](https://www.strikingly.com/)

## 4\. Pour aller plus loin

Installe ces outils et sers-t'en ! Teste des outils similaires, choisis ton préféré, fais de la veille pour en connaitre d'autres tout aussi pratiques. L'objectif est de sortir des sentiers battus, et d'utiliser ceux qui te feront gagner du temps que tu pourras alors consacrer à des tâches bien plus agréables.

# Cours : Faire de la veille : comment se tenir informé des actualités techniques ?

## 1\. Introduction

Comme tu le sais sans doute, le monde de la tech évolue très rapidement. Il est donc nécessaire de faire régulièrement de la veille pour ne pas rester à la traîne. Jette donc un oeil à ces quelques sites conseillés par la maison ! Ils t'aideront à te tenir au courant de l'actu dans le domaine. Nous les avons rassemblés en 4 catégories :

*   Les produits sympas du moment.
*   Les actualités techniques avec des articles simples.
*   Les actualités de la tech en général.
*   Les actualités des startups.

## 2\. La ressource

### 2.1\. Les produits sympas du moment

#### 2.1.1\. Product Hunt

[Product Hunt](https://www.producthunt.com/) est une plateforme où les utilisateurs viennent proposer leurs "trouvailles" : des applications / sites / produits récemment découverts. Le public est essentiellement composé de jeunes cadres urbains dynamiques de la tech, donc attends-toi à y découvrir ce qui existe de plus hype ! Product Hunt est tellement connu dans cet univers que des milliers de startups se battent pour être bien classées sur le site. Tu pourras y dénicher toutes les apps cools avant même qu'elles ne deviennent connues. C'est un excellent outil pour découvrir les futurs sites / applications / produits sympa.

### 2.2\. Les actualités techniques

#### 2.2.1\. HackerNews

Malgré son site au style austère faisant passer [Reddit](https://www.reddit.com/) pour un festival de couleurs, [Hacker News](https://news.ycombinator.com/) est une des références en termes d'actualité technique. Ce site est conçu par l'équipe de Y Combinator pour aider sa communauté (et plus) à partager les dernières actu du monde de la Tech.

Petite astuce : je ne vais pas souvent sur Hacker News, mais je me suis inscrit à leur [newsletter](https://hackernewsletter.com/) qui envoie une fois par semaine leurs meilleurs liens. C'est un indispensable.

#### 2.2.2\. Hacker Noon

[Hacker Noon](https://hackernoon.com/) est un blog hébergé sur [Medium](https://medium.com/) qui traite de l'actualité technique de manière simple et pédagogique. Ils proposent plein d'articles tutoriels sur des langages de programmation et font l'effort de vulgariser des concepts compliqués. C'est un excellent site pour qui sait un peu coder et souhaite continuer à comprendre les enjeux des développeurs de l'ère moderne.

### 2.3\. Les actualités de la tech en général

#### 2.3.1\. Planet

[Planet](https://www.getplanet.eu/) est une newsletter envoyée 2-3 fois par semaine. Elle s'arrête sur certains points de l'actualité technologique en prenant le temps d'expliquer ce qui se passe. Ça se lit bien et permet d'être rapidement à la page concernant les dernières infos du monde de la tech.

### 2.4\. Les actualités des startups

#### 2.4.1\. Techcrunch

[TechCrunch](https://techcrunch.com) est un blog traitant de l'actualité des startups. C'est le leader mondial du genre.

#### 2.4.2\. Maddyness

[Maddyness](https://www.maddyness.com/) est LE site français le plus connu concernant l'actu des startups.

## 3\. Points importants à retenir

Pour éviter de te submerger de sites et te filer une indigestion (du style "je m'abonne à tout mais je ne lis rien"), nous préférons t'en donner peu pour te permettre de faire de la veille sans te noyer. Si tu ne devais retenir que 3-4 noms, les voici :

*   [Product Hunt](https://www.producthunt.com/) pour connaître les actualités des produits sympa.
*   [Planet](https://www.getplanet.eu/) pour se mettre au fait des enjeux de la tech à haut niveau.
*   [HackerNewsletter](https://hackernewsletter.com/) pour savoir quelles sont les technologies qui prennent le devant.

## 4\. Pour aller plus loin

Si tu fais l'effort de parcourir régulièrement ces magazines, d'ici quelques mois tu auras une connaissance de l'univers tech qui te vaudra quelques compliments bien mérités 😇

# Cours : Tuto : installation d'une machine virtuelle pour The Hacking Project

## 1\. Introduction

Ce tutoriel te servira si tu souhaites faire tourner ton environnement de travail sous une machine virtuelle. Il a été réalisé par un corsaire de la session 10 : Olivier. En guise de mission moussaillon, Olivier a réalisé un tutoriel pour permettre à la communauté future de pouvoir faire une installation de Linux sans avoir à tout désinstaller. C'est aussi ça THP : la contribution à la communauté, le partage, et une formation qui vit avec ses élèves. Bref, voici le tutoriel.

Nous allons aborder la marche à suivre, pas à pas, de la mise en place d’un environnement de développement sur Windows 10, au travers d’une machine virtuelle.

Par machine virtuelle, nous entendons un logiciel qui te permettra d’exécuter un système d’exploitation Linux à l’intérieur même de ta session Windows 10\. En gros, c’est un logiciel qui permet de travailler sur un environnement Linux pour suivre THP en parallèle de ton environnement Windows 10 classique.

## 2\. Les ressources

### 2.1\. Ce qu’il faut savoir

Le cursus de THP ne sera pas gourmand en ressources matérielles, tu n’as pas besoin d’un PC de compétition pour atteindre avec brio ton statut de corsaire ! De fait, suivre THP au travers d’une machine virtuelle, ou VM, est tout à fait possible, à condition de respecter certaines étapes et de comprendre les limites de la solution.

#### 2.1.1\. Pour qui ?

Si au quotidien tu as besoin d’utiliser ton environnement Windows pour faire telles et telles tâches, le dual-boot ne sera peut-être pas optimal pour toi. De même, remplacer purement et simplement ton système d’exploitation par Linux ne te sera pas d’une grande aide pour utiliser des apps Windows. Enfin, peut-être que l’envie et/ou le besoin d’investir dans un nouveau PC sous Linux dédié uniquement au code n’est pas encore ta priorité du moment.

Pour ces différentes raisons, un environnement de développement virtuel peut-être la solution idéale pour toi.

#### 2.1.2\. Mon PC est-il assez puissant ?

Une VM est un logiciel qui permet l’émulation d’un autre système d’exploitation, à partir de ton Windows 10 natif, c’est-à-dire celui qui est installé sur ton PC. Ton PC fera donc tourner Windows 10, et celui-ci fera tourner la distribution Linux que tu souhaites utiliser pour THP au travers de la VM.

La VM est donc ni plus ni moins qu’un second ordinateur qui tourne en local par émulation du système d’origine. De fait, les performances accessibles par une VM par rapport aux ressources qui lui seront allouées, seront bien plus faibles par rapport à ce qu’il est possible d’atteindre en natif. Cependant, pour suivre THP dans de (très) bonnes conditions, l’essentiel n’est pas d’avoir un monstre de puissance mais une machine stable et efficace. Actuellement, tu peux donc avoir un ordinateur qui se « traîne » dans la vie de tous les jours... et si c’est le cas, rendez-vous à la section « 3.1.3 Améliorer mes performances ».


>#### 🚀 ALERTE BONNE ASTUCE
>
>Si tu souhaites connaître la configuration matérielle de ton ordinateur, rends-toi dans les paramètres de ton ordi, c’est la « roue dentée » au-dessus du bouton marche-arrêt de ton PC dans le menu démarrer de celui-ci. Ensuite, clique sur « Système » sur la page d’accueil de la fenêtre Paramètres, puis dans la barre de défilement à gauche, c’est le dernier choix « Informations Système ». Ici, tu sauras combien de RAM au total ton PC dispose, ainsi que son processeur.
>
>Pour connaître de quelle capacité de stockage libre ton disque dur dispose encore, rends-toi dans « Ce PC » depuis le menu déroulant de gauche de l’ « Explorateur de fichiers ». Tu y trouveras les différents disques durs installés et leur état d’occupation actuel.

Cette émulation utilisera donc une partie des ressources matérielles de ton PC :

1.  son processeur
2.  sa mémoire vive ou RAM
3.  son disque dur

Tout d’abord, tu devras allouer une part de ton disque dur à la VM et celle-ci, tant que la VM sera installée sur ton ordinateur, ne pourra pas être utilisée à d’autres fins : elle sera inaccessible. Nous conseillons un minimum de 10Go. Assure donc toi que cela est possible grâce à l’astuce précédente.

Ensuite, tu devras faire de même avec ta mémoire vive : la part allouée restera inaccessible au reste de tes logiciels sur Windows 10 tant que la VM sera en route. Mais pas d’inquiétude, une VM peut se mettre à l’arrêt comme tout logiciel. Le minimum de mémoire que nous recommandons est de 2Go, si tu as au total 4Go de RAM. Si ton PC possède plus de RAM installée, comme la plupart des ordinateurs modernes, je te conseille d’en allouer plus, et ce jusqu’à 4Go. En effet, après ce cap plus aucune différence ne se fera sentir dans l’utilisation de la VM que tu feras durant ton cursus de moussaillon.

Enfin, ton processeur doit être assez puissant pour supporter deux systèmes à la fois. Mais pour le savoir, rien de mieux que d’essayer ! Si ton ordinateur a moins de dix ans, ça devrait le faire 😉.

#### 2.1.3\. Améliorer les performances de ton PC

Aujourd’hui, ton PC est peut-être vraiment lent dans son utilisation quotidienne et c’est peut-être parce qu’il n’est plus au goût du jour. Cependant, c’est peut-être aussi dû à une surconsommation de ses ressources !

Dans ce dernier cas, avant d’investir, nous te conseillons de vérifier quels logiciels sont installés et lesquels sont en route en permanence. Tu pourras le faire grâce à l’intermédiaire de [CCleaner](https://www.ccleaner.com/ccleaner/download/standard ), qui est fort utile dans sa version gratuite.

CCleaner te permettra en plus de vider l’historique et les fichiers en cache, :

1.  d’avoir la liste complète des logiciels installés et de pouvoir désinstaller ceux qui te sont inutiles / indésirables (et oui, c’est fort possible !).
2.  d’avoir la liste complète des logiciels qui se lancent au démarrage de ton ordinateur, souvent sans nécessité !

Ces deux éléments sont accessibles depuis l’onglet « Tools », dans la liste de gauche. Puis depuis, la liste de gauche, les onglets « Uninstall » et « Startup » te permettront respectivement de désinstaller les logiciels indésirables et d’annuler le lancement au démarrage de la machine (par exemple Skype). Cependant, nombre d’entre eux te seront inconnus, et avant toute action renseigne toi en recherchant leur nom sur Google.

### 2.2\. Installation de la VM

Nous allons tout d’abord s’assurer que ton ordinateur accepte la virtualisation sur ton système puis nous allons installer VirtualBox, un logiciel facile d’accès, gratuit et open-source !

#### 2.2.1\. Le BIOS

Tout d’abord, vérifions que ton ordinateur autorise la virtualisation. Pour cela tu vas te rendre dans son BIOS 😉 ! Suis donc ces différentes étapes :

1.  Redémarre ton PC
2.  Avant d’arriver à l’écran bleu de démarrage Windows, appuie sur la touche ou la combinaison de touches spécifique à l’accès à ton BIOS. Celle-ci varie en fonction des fabricants et bien sûr Google est ton ami 😉. Mais le plus souvent ce sont les touches ESC, F1, F2 ou F10 qui fonctionnent.
3.  A présent, grâce aux touches directionnelles et ENTER navigue tel le courageux moussaillon que tu es dans ce merveilleux BIOS!
4.  Puis, en fonction de ce qui se présente, rends-toi dans l’onglet avec l’un des noms suivants:
    *   « Security »
    *   « Advanced »
    *   « System Configuration »
    *   Si tu ne trouves toujours pas, cherche sur internet la méthode correspondant à la marque de ton d’ordinateur.
5.  Sélectionne ensuite « Virtualization Technology » ou « Virtualization » que tu passes à « Enable »
6.  Quitte ton BIOS en sauvegardant et redémarre ton ordinateur s’il ne le fait pas de lui-même.


>#### ⚠️ ALERTE ERREUR COMMUNE
>
>Il est possible que l’accès à ton BIOS et/ou la sauvegarde des modifications nécessitent un mot de passe que toi, ou le précédent propriétaire, a renseigné lors de la première mise en route de ton PC. Nous te souhaitons donc de l’avoir si la virtualisation est interdite pour les paramètres de ton BIOS.

#### 2.2.2\. VirtualBox

Je te laisse télécharger et installer le logiciel à cette [adresse](https://www.virtualbox.org/wiki/Downloads). Choisis le « Windows hosts package ».

Comme à chaque installation, tu auras des choix à faire tels que la localisation de l’installation sur ton disque dur et d’autres options. Nous te conseillons de conserver les sélections par défaut de VirtualBox et d’attendre tranquillement le message de fin du processus.

#### 2.2.3\. Xubuntu

Nous te recommandons ensuite de choisir un OS qui ne sera pas gourmand en ressources et donc parfait pour une VM. Xubuntu par exemple est un excellent candidat. C’est un dérivé de Ubuntu construit sur le noyau Linux. Cet OS a en effet spécialement été créé pour être utilisé en tant qu’environnement de programmation : il est efficace, stable et tu peux le télécharger à l’adresse [suivante](https://xubuntu.fr/) .

#### 2.2.4\. Création de ta nouvelle machine virtuelle

Lance VirtualBox et clique sur « Nouvelle » depuis l’onglet « Machine ». Nomme la « Xubuntu », indique le « Type » à « Linux » et la « Version » à « Ubuntu (64-bit) ». Ne modifie pas le dossier de la machine. Enfin, appuie sur « Suivant ».

Sélectionne la RAM que tu souhaites allouer à la VM, comme vu précédemment, puis « Créer un disque virtuel ». Sélectionne ensuite l’option « VDI », puis « Dynamiquement alloué » et enfin indique le nombre de Giga-octets que tu souhaites, 10 étant le minimum recommandé. Clique sur « Créer ».

Ta VM apparaît maintenant dans le menu de VirtualBox. Clique droit dessus, va dans « Configuration » puis « Système ». Dans l’onglet « Processeur » passe le nombre de processeurs à deux.

Toujours dans les paramètres de configuration, va dans l’onglet « Stockage ». Clique sur « Vide » en dessous de « Contrôleur : IDE » et dans la colonne « Attributs » clique sur l’icône de disque bleu et puis sur « Choisissez un fichier de disque optique virtuel ». Il faudra y indiquer le fichier en .iso que tu as reçu en lançant le téléchargement de Xubuntu. Quitte la fenêtre de configuration de la VM grâce à « OK » pour sauver les changement que tu viens d’opérer.

A présent clique sur « Démarrer » en sélectionnant ta VM « Xubuntu ». L’installation de l’OS se lancera et nous te conseillons de ne pas toucher aux paramètres par défaut.


>#### 🚀 Pas de panique
>
>Ce qui se passera dans ta VM ne pourra pas affecter ton ordinateur. Si quelque chose « casse », tu pourras tout réinstaller de zéro sans que cela ne mette en danger tes fichiers stockés sur ton PC. Également, les virus et autres malwares y resteront confinés !

#### 2.2.5\. Pimp my VM !

Une VM est un environnement clos, dans lequel tu pourras tester sans peur tout ce que tu veux. Mais pour plus de praticité, et parce que tu seras responsable et ne feras rien qui ne mettra en péril ton PC et tes projets de moussaillon, nous allons autoriser quelques échanges entre ton Windows 10 et ta VM « Xubuntu ».

Met en route ta VM et en haut de la fenêtre, clique sur « Ecran ». Dans cet onglet tu pourras régler la résolution de l’écran que tu utilises pour afficher la VM : clique sur « Taille d’écran automatique » pour plus de praticité.

Ensuite, clique sur « Périphériques ». Et configure le « Presse-papier partagé » et le « Glisser-déposer » à « Bidirectionnel ». Tu pourras maintenant, depuis ton Windows 10 ou bien depuis ta VM effectuer des Drag’n Drop de fichiers et des copier-coller dans un sens comme dans l’autre !

## 3\. Points importants à retenir

Une machine virtuelle est un outil très puissant qui te permettra de suivre THP dans les meilleures conditions tout en conservant ton ordinateur sous Windows 10 intact. C’est maintenant ton environnement de développement dédié à THP, dans lequel tu programmeras et sauvegarderas tes projets.

Cependant, des ralentissements peuvent survenir : nous te conseillons de ne pas faire tourner trop de programmes en parallèle sur ton Windows 10.

Si tu crains qu’un drame ne survienne et que ta VM ne sois plus utilisable le jour où il te faut rendre un projet validant, il est possible de faire des restaurations et des clones de celle-ci. C’est bien évidemment à utiliser avec parcimonie car cela prend beaucoup de place sur le disque dur.

Il peut également arriver que ta VM soit illisible, trop pixelisée, avec uniquement des gros boutons, etc… Et bien sache que cela est un simple problème de résolution d’écran : modifie la résolution de la VM comme expliqué précédemment pour qu’elle coïncide avec celle de ton écran d’affichage.

# Cours : Tuto : mise en place de WSL pour The Hacking Project

## 1\. Introduction

Ce tutoriel te servira si tu souhaites faire tourner ton environnement de travail sous Windows Subsystem for Linux. Il a été réalisé par un corsaire de la session 10 : Julien. En guise de mission moussaillon, Julien a réalisé un tutoriel pour permettre à la communauté future de pouvoir faire une installation de Linux sans avoir à tout désinstaller. C'est aussi ça THP : la contribution à la communauté, le partage, et une formation qui vit avec ses élèves. Bref, voici le tutoriel.

Cette ressource peut te permettre de suivre THP en utilisant le Sous-système Linux Ubuntu pour Windows 10 (En anglais : Windows Subsytem Linux, abréviation : WSL)! et ainsi :

*   éviter l'achat d'un nouveau PC que tu n'utiliseras plus après THP
*   de te prendre la tête avec les machines virtuelles
*   éviter les crises paniques liées à ta phobie de faire un dualboot (en particulier à causes du partitionage du disque dur)

C'est simple et rapide à installer !... Mais il y aura quelques règles à respecter ! lis bien la ressource jusqu'au bout ! ..... Oui ! jusqu'au bout ! ..... Oui ! toutes les lignes !

Toute la formation THP est compatible de cette architecture, mis à part le cours bonus sur la gem Watir (bot qui se balade sur internet via un vrai navigateur web)

## 2\. Historique

Jusque fin 2019, plusieurs architectures Hard/OS étaient proposées pour réussir THP:

*   SingleBoot Linux
*   DualBoot Linux/Windows
*   SingleBoot Windows + Machine virtuelle Linux

De quoi en refroidir plus d'un avant même d'avoir commencé ! Voici une nouvelle architecture compatible Windows 10 et THP éprouvée à la session 10 (fin 2019) :

*   BootOnly Windows 10 + WSL Ubuntu

## 3\. Installation de WSL Ubuntu

### 3.1\. Introduction

Cette ressource a été écrite pour Windows 10\. Tout autre Windows (3.11 et autres ...) n'a pas été testé dans cette ressource

### 3.2 Installer WSL

La [ressource](https://docs.microsoft.com/fr-fr/windows/wsl/install-win10) de Microsoft sur Windows Subsystem Linux est claire et concise, suis là à la lettre

>#### ⚠️ ALERTE ERREUR COMMUNE
>
>Clique bien sur `Exécuter en tant qu'administrateur` et non pas juste `ouvrir`

### 3.3 Installer la distribution Ubuntu

À la date où j'écris cette ressource, sont disponibles dans le Microsoft Store

*   Ubuntu
*   Ubuntu 18.04 LTS
*   Ubuntu 16.04 LTS

J'ai choisi la distribution Ubuntu (Ma config : Windows 10 édition famille 64 bits) et n'ai pas testé les autres

### 3.4 Initialisation d’une distribution nouvellement installée

Là aussi, la [ressource](https://docs.microsoft.com/fr-fr/windows/wsl/initialize-distro) Microsoft est bien faite.

## 4\. Utiliser WSL Ubuntu

### 4.1 Création de mon premier Dossier et Fichier avec WSL

A partir du menu démarrer lance l'application Windows Ubuntu. Cette application correspond au terminal Linux. Saisi les commandes suivantes :
```bash
$ mkdir dossierlinux
$ cd dossierlinux
$ touch fichierlinux.md 
```
Félicitation ! Tu viens de créer tes premiers dossiers et fichiers linux via WSL Ubuntu

### 4.2 Edition de mon fichier Linux depuis Windows

#### 4.2.1 Installer d'un éditeur de code/texte sous Windows

Installe la version Windows de l'éditeur de code [Visual Studio Code](https://code.visualstudio.com/download). Il est probable que ça marche aussi avec d'autres éditeurs, mais ça n'a pas encore été testé.

#### 4.2.2 Trouver les fichiers linux avec l'explorateur Windows

L'application Windows Ubuntu enregistre tous les fichiers et dossiers dans un chemin qui ressemble à celui-ci dessous :

```bash
C:\Users\USER\AppData\Local\Packages\CanonicalGroupLimited.UbuntuonWindows_79rhkp1fndgsc\LocalState\rootfs\home\
```

>#### ⚠️ ALERTE ERREUR COMMUNE
>
>Il est possible que le chemin soit différent de celui cité, en particulier pour le `USER`

>#### 🚀 ALERTE BONNE ASTUCE
>
>Pour trouver le bon chemin rapidement, dans l'explorateur Windows recherche dans le dossier AppData le fichier fichierlinux.md que tu viens de créer à l'instant. Tu sais maintenant où WSL Ubuntu stocke les données.
#### 4.2.3 Edition des fichiers WSL Ubuntu depuis Windows

Ouvre tout le dossier dossierlinux/ avec l'éditeur de texte. Va sur le fichier fichierlinux.md Fais les modifications que tu souhaites, enregistre. C'est fini !

>#### ⚠️ ALERTE ERREUR COMMUNE
>Depuis Windows on ne s'autorise qu'à modifier le contenu des fichiers

## 5\. Points importants à retenir

WSL Ubuntu + Visual Studio Code c'est top !

Windows gère ses fichiers d'une façon, WSL Ubuntu les gère d'une autre. En découle des règles d'utilisation suivantes :

*   Règle 1 : Toutes les créations et suppressions des fichiers et dossiers Linux doivent être effectuées depuis le terminal Ubuntu... TOUTES !
*   Règle 2 : Tous les changements de noms et déplacements de fichiers et/ou dossiers Linux doivent être effectués depuis le terminal Ubuntu... TOUS
*   Règle 3 : Ne jamais enfreindre les règles 1 et 2

>#### ⚠️ ALERTE ERREUR COMMUNE
>
>Considère un téléchargement comme une création de fichier. Utilise la fonction `wget` pour télécharger dans ton WSL Ubuntu

## 6\. Pour aller plus loin

Si tu as choisi Visual Studio Code, pense à le personnaliser (indentation à 2 espaces, add-on pour fichier ruby, etc.)

N'hésite pas à compléter cette ressource (pimp terminal par exemple, etc )

Enjoy !

# Projet : Réalisation d'une landing page

## 1\. Introduction

Là voilà, la fameuse Landing Page ! Le projet de toute une semaine, au cours de laquelle tu auras vu :

*   Les bases de HTML / CSS.
*   La façon de mettre un site en ligne.
*   Bootstrap et les frameworks pour concevoir des pages rapidement.

Avec les notions de design et de marketing que nous t'avons données aujourd'hui, te voici fin prêt à réaliser la page d'accueil de ta startup / association / entreprise. Tu vas devoir lui donner un _CTA (call to action)_ fonctionnel, puis la mettre en ligne. Allons-y !

## 2\. Le projet

Pour ce projet, nous allons te demander de designer, coder, puis mettre en production une landing page. Voici la marche à suivre détaillée :

*   Choix de l'organisation que tu veux promouvoir.
*   Choix de l'objectif de la page et de son call to action.
*   Design de la page.
*   Code de la page.
*   Mise en production.

### 2.1\. Choix de l'organisation

Pour cette page, nous te demandons de choisir une organisation concrète sur laquelle travailler. Cela permettra de mieux te projeter et de proposer un meilleur rendu. Voici quelques possibilités :

*   Ton association étudiante.
*   Une association que tu connais et apprécies.
*   Ta future startup qui va tout déchirer.
*   Ton entreprise.
*   L'association / entreprise d'un(e) de tes proches.
*   Le projet d'un co-moussaillon avec qui tu vas co-travailler pour ce projet.
*   L'entreprise à qui tu as vendu cette page (cela peut se négocier entre 500€ et 2500€ en fonction de tes capacités en négociation et de ta volonté à faire raquer l'entreprise)

Une fois l'organisation choisie, passons à la reflexion sur les fonctionnalités de ta page.

### 2.2\. Objectif : quel CTA

Souviens-toi : "Avant de foncer tête baissée dans le code, prends le temps de te poser et de réfléchir à ce que ta page doit faire". En effet, tu ne vas pas coder la page d'un restaurant de la même façon que celle d'une startup qui lance son produit dans 3 mois. Pour la première, tu ferais un site vitrine affichant un menu, pour l'autre tu proposerais une inscription à une mailing list pour être tenu au courant du lancement.

Voici donc une liste non exhaustive de ce que tu peux faire avec une page simple :

*   Un [bouton](https://stackoverflow.com/questions/17219688/href-tel-and-mobile-numbers) pour appeler un numéro défini.
    *   Ce peut être utile pour faire une demande de réservation pour un restaurant, par exemple.
*   Un bouton "Nous suivre sur les réseaux sociaux" qui redirige vers une page Facebook (notamment).
    *   Très pratique pour une organisation qui utilise les réseaux sociaux comme principal canal de communication (une association).
*   Un formulaire pour s'inscrire à une mailing list, comme [celle de Mailchimp](https://mailchimp.com/fr/help/add-a-signup-form-to-your-website/).
    *   Très pratique pour tenir les personnes au courant du projet ou envoyer des offres promotionnelles.
*   Plein d'autres CTAs sont possibles, tout dépend ce qui le plus pertinent pour ton organisation.

### 2.3\. Design de la page

Avant de te mettre à coder, il faut que tu définisses à quoi va ressembler ta page et quels éléments y seront. Il y a un truc qu'on aime bien à THP : éviter aux moussaillons de leur faire réinventer la roue. Pour les pages, inspire-toi de tous les templates et thèmes qui existent pour voir :

*   Quelles sont les parties importantes à mettre dans une page.
*   Quelles parties seront les meilleures pour ta page.

Ce travail d'inspiration est très important dans l'univers du design produit : au lieu de vouloir se prendre la tête à tout refaire, pourquoi ne pas s'inspirer d'entreprises ayant investi des millions d'euros dans ce domaine et qui savent ce qui marche ? Va donc parcourir le net pour trouver ton bonheur et conçois ta page en fonction.

Enfin, avant de coder, tu vas être confronté à deux choix :

*   Option **des p'tits malins** : tu prends un thème déjà existant, tu enlèves / modifies les parties et zoupla, ta page est prête !
    *   Avantages : ta page est prête rapidement, et elle sera belle.
    *   Défauts : manque d'originalité, pas entièrement customisable.
*   Option **customisation** : tu utilises Bootstrap de base (ou une surcouche à la [Bootswatch](https://bootswatch.com/)) et tu effectues l'intégralité de la page.
    *   Avantages : ce sera TA page que TU auras codée du début à la fin, et tu en seras fier.
    *   Défauts : à moins d'être bon en design, ta page sera moyenne, voire moche, et ne sera donc pas très attrayante. Réinventer la roue, c'est long, et souvent contre-productif.

Le choix t'appartient ☺

### 2.4\. Code de la page

Les préparatifs sont finis, passons au code ! Prépare un repository GitHub, un autre sur ton ordinateur, et c'est parti !

### 2.5\. Mise en production

Une fois ta page codée et ton visage illuminé d'un fier sourire, il est temps de faire profiter la terre entière de ton travail (quel intérêt, sinon ?). Plusieurs solutions s'offrent à toi :

*   Un nom de domaine personnalisé, généralement en `nomdetonorganisation.com` ou `nomdetonorganisation.fr` ou autre (`.co`, `.org`, etc) (indispensable si tu veux que les recherches Google de `Nom de ton organisation` renvoient vers ton site).
*   Une option comme Surge ou GitHub Pages pour juste le mettre en ligne.

Idem, nous te laissons choisir ce qui t'arrange le mieux, puis mettre le site en ligne.

## 3\. Rendu attendu

Une jolie page de présentation de ton organisation, avec un objectif, et en ligne !

# Projet : Tes devoirs : faire les installations pour la formation

## 1\. Introduction

Pour la formation, tu devras effectuer quelques préparatifs. En effet, la plupart des programmes que nous utiliserons pendant ces 11 semaines requièrent un ordinateur proposant un système d'exploitation à coeur Unix. C'est à dire : **il est impossible de faire la formation avec Windows en tant que tel** : il te faudra installer soit WSL, soit Linux, ou encore macOS sur ton ordinateur.

Dans cette ressource, nous allons voir ensemble comment faire pour avoir un ordinateur compatible avec la formation. Plusieurs solutions s'offrent à toi, chacune avec ses avantages et ses défauts :

*   Siroter un thé si tu as déjà Linux ou macOS sur ton ordinateur.
*   Une machine virtuelle avec Linux dessus.
*   Installer Linux sur ton ordinateur en dual boot ou only boot.
*   Windows Subsystem for Linux.
*   Acheter un ordinateur pour la formation.

Nous te recommandons de faire ce projet avec d'autres moussaillons : vous pourrez ainsi mutualiser vos erreurs, et résoudre ensemble vos problèmes.

## 2\. Le projet

Linux est un système d'exploitation créé en 1991 par Linus Torvald (le créateur de Git). Il possède un coeur Unix, contrairement à Windows basé sur MS-DOS. Tu pourras retrouver un peu plus d'informations sur Linux dans [l'excellent cours de Mathieu Nebra](https://openclassrooms.com/courses/reprenez-le-controle-a-l-aide-de-linux/mais-c-est-quoi-linux) à ce sujet.

Linux propose plein de versions différentes, nommées _distribution_, qui ont chacune leur intérêt. Par exemple il existe des distributions idéales pour [faire tourner des serveurs](https://www.centos.org/). En ce qui te concerne, nous te conseillons de passer par [Ubuntu](https://www.ubuntu.com/), ou [Mint](https://linuxmint.com/), excellentes distributions stables, modifiables, robustes, et très sécurisées.

Si tu possèdes un ordinateur avec Windows, nous te proposons 4 solutions pour faire tourner Linux sur ton futur ordinateur :

*   Une machine virtuelle : un programme qui émule un système d'exploitation, et peut donc faire tourner Linux dessus.
    *   Avantages : Facile à installer ; pas de risque de casser ton ordinateur.
    *   Inconvénients : Ça demande une machine puissante car tu fais tourner deux ordinateurs sur une seule machine ; Elle peut aussi planter en cours de formation. Comme ça arrive généralement au pire moment, réserve-toi une nuit blanche ou deux d'avance, ou pire : un abandon contraint lors d'un bug sur ta machine virtuelle.
*   Installer Linux en dual boot / only boot : installer Linux directement sur ton ordinateur, soit en effaçant tout, soit en divisant ton disque dur en deux pour installer Linux à côté de Windows.
    *   Avantages : tu as Linux qui tourne à merveille sur ton ordinateur. Ce dernier tournera plus vite comparé aux autres solutions. Il s'agit du meilleur choix pour les amateurs de l'Open Source.
    *   Inconvénients : tu devras bidouiller dans les entrailles de ton ordinateur et être attentif pendant l'installation. Avec certaines machines, il te faudra bidouiller encore plus pour tout installer. C'est la technique la plus longue...
*   Windows Subsystem for Linux (attention, ceci n'est disponible que pour Windows 10) : il est possible d'emuler Linux sur Windows 10 avec WSL.
    *   Avantages : c'est réglé en 10 minutes d'installation !
    *   Inconvénients : c'est la technique des experts, étant donné que tu ne devras te servir de ton ordinateur qu'avec le terminal pendant toute la formation.
*   Acheter un ordinateur pour la formation : c'est plutôt équivoque ☺
    *   Avantages : c'est plié très rapidement.
    *   Inconvénients : l'addition est beaucoup plus salée (entre 150€ et 1200€).

### 2.1\. Une machine virtuelle

L'installation d'une machine virtuelle se passe en quatre étapes :

1.  Télécharger Linux et un logiciel de virtualisation (type VirtualBox)
2.  Installation.
3.  Paramétrages.
4.  Quelques astuces.

Pour ceci, nous te recommandons de suivre l'excellent pas à pas de notre corsaire Olivier plus haut dans les ressources du jour.

### 2.2\. Dual Boot / Only boot

#### 2.2.1\. Le only boot

Cette technique consiste à tout virer sur l'ordinateur actuel que tu as, et de mettre Linux à la place. C'est assez simple, puisqu'il te suffit globalement de faire "oui je veux tout effacer pour installer Linux" et hop, à toi la gloire ! De plus, tu peux facilement acheter [un ordi portable](https://www.leboncoin.fr/informatique/offres/ile_de_france/?th=1&q=ordinateur%20portable) sur LeBonCoin, et tout effacer pour lui coller Linux.

Voici [un tutoriel](https://www.youtube.com/watch?v=kIhFFofixpo) expliquant comment installer simplement Linux sur son ordinateur.  
À un moment, le vidéaste dira qu'il faut graver Linux sur un CD (lol), et booter son ordinateur avec. Puisque nous sommes en 2019, les graveurs sont passés de mode, et il est très facile de le faire avec une clé USB ( [voici un tuto qui permet d'avoir une clé USB bootable Linux](https://www.tech2tech.fr/creer-une-cle-usb-bootable-avec-rufus/)). Il faut ensuite redémarrer son ordinateur pour qu'il utilise la clé USB (et non pas Windows) pour effectuer l'installation de Linux. [Voici un tutoriel expliquant le démarrage du BIOS](https://www.youtube.com/watch?v=NsYty-Qbs04&t=255s). Comme démarrer son ordinateur sur le BIOS est différent pour chaque carte mère (des fois c'est F2, des fois F8, etc), fais une recherche Google `access bios [modèle_ordinateur]` pour trouver la bonne combinaison.

#### 2.2.2\. Le dual boot

L'installation est assez similaire à la précédente. Elle consiste à avoir deux OS sur ton ordinateur : Windows, et le Linux que tu vas installer. Il te faudra diviser ton disque dur (ou SSD) en deux partitions : une pour Windows, et une pour Linux. Voici [une vidéo tutoriel](https://www.youtube.com/watch?v=qNeJvujdB-0) montrant comment installer Linux en dual boot.

### 2.3\. Windows Subsystem for Linux

Pour ceci, nous te recommandons de suivre l'excellent pas à pas de notre corsaire Julien plus haut dans les ressources du jour.

### 2.4\. Acheter un ordinateur

Si tu penses que tu vas galérer, ne te prends pas la tête. Une simple recherche LeBonCoin "[portable Linux](https://www.leboncoin.fr/annonces/offres/ile_de_france/?th=1&q=portable%20linux)" ou même sur [CDiscount](https://www.cdiscount.com/informatique/r-pc+portable+linux.html#_his_) te fera trouver ton bonheur pour une ou deux petites centaines d'euros.

## 3\. Rendu attendu

Un ordinateur avec Linux dessus prêt pour la formation :)
