![Texte de remplacement si l’image ne se charge pas](https://www.meosis-blog.fr/wp-content/uploads/sites/9/2016/03/logiciel-de-programmation.jpg)

# Les bonnes pratiques du code informatique

Qu'est-ce qui caractérise un code "bien écrit" ?

Un algorithme, ou code "bien écrit" doit avoir les propriétés suivantes :

- Être facile à lire, pas soi-même mais aussi par les autres.
- Avoir une organisation logique et évidente.
- Être explicite, montrer clairement les intentions du développeur.
- Être soigné et robuste au temps qui passe.

Nous allons regarder un peu plus en détails chacune de ces caractéristiques.

## La code doit être facile à lire

Pour que le code soit facile à lire, il faut d'une part qu'il soit bien structuré et bien présenté, et d'autre part, que les noms des variables et des fonctions soient choisis avec soin.

Pour ce qui est de la structure et de la présentation, Python nous aide beaucoup car le langage impose beaucoup de choses qui nous "forcent" à bien présenter notre code. Par exemple, les blocs d'instructions du même niveau doivent être précédés du même nombre d'espaces, ce qui nous conduit naturellement à bien indenter notre code.

Dans d'autres langages, plus de libertés de présentation sont offertes au développeur, par conséquent, il convient de se forcer à respecter des conventions pour écrire le code le plus propre possible.


## Le code doit avoir une organisation logique et évidente

Ce point est plus délicat car nous avons souvent des solutions différentes pour résoudre le même problème. Il est donc normal qu'un code qui semble logique à quelqu'un semble "tordu" à son voisin.

Étant conscient de cela, il faut vous efforcer de trouver des solutions logiques aux problèmes que vous devez résoudre et d'éviter d'emprunter des chemins plus compliqués qui ne feraient que semer la confusion.

Par exemple, si l'on vous demande d'afficher tous les nombres de 1 à 10, il suffit de faire une boucle qui fait évoluer un compteur entre 1 et 10 et qui affiche, à chaque tour, la valeur de ce compteur. La solution qui consisterait à faire une boucle qui fait évoluer un compteur de 9 à 0 et qui afficherait à chaque tour le résultat de 10 - compteur fonctionne aussi mais est à proscrire car elle est "tordue".
Le code doit être explicite

Lorsque l'on écrit des algorithmes ou que l'on développe des programmes, on est parfois tenté de prendre des raccourcis car "on sait" que telle ou telle méthode permet de faire telle ou telle chose bien pratique.

Il n'est pas interdit de prendre ces raccourcis, mais il faut toujours prendre le soin d'expliquer, au moins à travers des commentaires, pourquoi on fait cela. C'est important à la fois pour permettre aux autres de comprendre pourquoi votre solution est astucieuse... mais aussi pour vous, au cas où vous ne vous souveniez plus de "pourquoi vous avez fait ça".

## Le code doit être soigné et robuste au temps qui passe

Lorsque l'on écrit du code, on a la fâcheuse tendance à s'arrêter dès que celui-ci fonctionne. C'est un tort ! Le code doit être entretenu. Cela signifie qu'il faut relire son code après l'avoir terminé, vérifié que l'on a bien supprimé les éléments obsolètes, vérifier que les commentaires sont à jour et cohérents avec le code conservé, etc...

Cette opération de "maintenance" du code est cruciale, mais elle est pourtant souvent négligée par beaucoup, ce qui peut poser des problèmes, notamment lorsque vous rencontrez un bug.

L'exemple le plus classique est celui-ci : vous implémentez une méthode tri qui permet de trier les éléments d'un tableau. Vous n'êtes pas satisfait du comportement de cette méthode lorsque vous l'utilisez depuis votre programme principal. Vous implémentez donc une autre méthode test qui utilise une autre stratégie pour trier les éléments du tableau. Cette méthode marche mieux. Vous l'utilisez donc dans votre programme principal. Votre programme fonctionne et vous passez à autre chose, sans penser à intégrer vos modifications proprement dans votre programme. Quelques jours plus tard, vous reprenez votre code et vous observez un bug. Vous pensez que cela provient du tri du tableau. Vous allez donc observer ce qui se passe dans tri. Après quelques heures de recherche, vous êtes furieux contre vous-même car vous réalisé enfin que la méthode tri n'est plus utilisée depuis longtemps dans votre code...

Croyez-le, les problèmes de ce type arrivent beaucoup plus souvent qu'on ne le pense... surtout quand on cherche à faire vite.


## C'est bien joli tout ça, mais coder proprement ça prend du temps !

C'est faux ! Il ne faut pas confondre vitesse et précipitation.

On a souvent tendance à penser que l'on perd énormément de temps à soigner son code, à le structurer correctement, à le réorganiser et à le documenter, mais c'est faux. Au contraire, on gagne du temps à faire tout cela.

Voici quelques explications pour vous en convaincre :

- Si vous adoptez les bonnes pratiques dès le début, vous faites déjà 50% du travail.
- Si le code est bien écrit, il est plus facile, et donc plus rapide à relire, et n'oubliez pas que vous passez plus de temps à lire votre code qu'à l'écrire... donc quand votre code est propre, vous vous faites gagner du temps.
- Si le code est logique et bien structuré, il sera plus facile de retrouver les bugs qu'il contient, et donc de l'améliorer..

Ce sont donc autant de raisons qui devraient vous convaincre qu'il est important d'être organisé, clair, méthodique et rigoureux quand vous développez.

## L'importance des commentaires

Les commentaires sont essentiels pour "éclairer" le code. Un commentaire est un texte qui est ignoré par l'ordinateur lorsqu'il exécute le programme, mais qui peut être lu par le développeur lorsqu'il lit le programme.

En Python, une ligne qui débute par le signe # est un commentaire. On peut aussi faire des blocs de commentaires, sur plusieurs lignes, en utilisant les triples guillemets.

Bien que les commentaires soient essentiels, il ne faut pas en abuser.

Un bon commentaire peut :

- Faciliter la lecture du code,
- Apporter une indication sur un choix de conception,
- Expliquer une motivation qui ne serait pas évidente,
- Donner un exemple pour permettre de mieux comprendre ce que fait le code.

Quelques exemples de mauvais commentaires :

- Un commentaire qui décrit un morceau de code qui n'existe plus,
- Un commentaire qui explique une évidence,
- Un commentaire sur plusieurs lignes pour expliquer une chose simple.
- Un commentaire sur l'historique des modifications d'un fichier. C'est parfois utile, mais dans la plupart des cas, il vaut mieux confier cette tâche à votre gestionnaire de versions qui fera le travail pour vous.

Attention : les commentaires ne doivent pas pallier un manque de clarté du code. Si vous avez besoin de commentaires pour cela, c'est probablement que vous pouvez améliorer votre code pour le rendre plus lisible. Essayez donc de le refactorer, c'est-à-dire de le ré-écrire, au moins partiellement, en l'améliorant.

Comme nous l'avons dit plus haut, les commentaires, tout comme le code, doivent être maintenus, c'est-à-dire qu'ils doivent évoluer avec le code, et disparaître si le code disparaît. Par conséquent, il faut veiller au bon dosage de vos commentaires, de sorte à ne pas alourdir inutilement votre travail de maintenance.


## Comment nommer les choses ?

Les noms que vous choisissez pour vos variables et vos fonctions vont grandement contribuer à la lisibilité de votre code.  

La première règle est donc de choisir des noms de variables prononçables et faciles à retenir.

Vous devez choisir des noms de variables explicites pour vous mais aussi pour les autres.

Par exemple, "a" est bien moins explicite que "adresseClient". De même, "lf" est moins explicite que "largeurFenetre". Pensez également que vous serez probablement amenés à chercher vos variables dans votre code avec un outil de recherche. À votre avis, combien d'occurrences de "a" allez vous trouver ? Et combien d'occurrences de "adresseClient" ?

Évitez également de choisir des noms de variables qui induisent un contre-sense. Par exemple, si vous écrivez matrice=8, on pourrait penser que la variable est une matrice, or, il s'agit clairement d'un entier.

Évitez également les noms de variable qui n'ont pas de sens, comme plop, surtout si vous en utilisez plusieurs dans la même portion de code. Vous risquez de vous perdre dans les noms et donc d'introduire inutilement des bugs dans votre code.

Ne trichez pas non plus quand vous choisissez vos noms de variables. Dans la plupart des langages de programmation, certains mots sont "réservés" car ce sont des instructions du langage. Par exemple, en Python, on ne peut pas nommer une variable if ou list car ce sont des mots réservés du langage. Si vous pensez avoir besoin de ces mots pour nommer vos variables, ne trichez pas en écrivant iff ou llist, vous risqueriez de vous perdre dans vos propres astuces.

La plupart des langages imposent des règles pour le choix des noms de variables. Par exemple, en Python, un nom de variable ne peut pas commencer par un chiffre (il y a d'autres règles). En plus de ces règles imposées par les langages, essayez de ne pas utiliser des caractères qui pourraient porter à confusion. En particulier, les caractères o 0 O l i et 1 peuvent se ressembler fortement, voire être identiques en fonction de la police de caractères utilisée pour l'affichage à l'écran.

Enfin, essayez d'être cohérents lorsque vous choisissez vos noms de variables. Par exemple, si vous décidez d'utiliser le français pour nommer vos variables, utilisez le français tout du long, n'alternez pas avec l'anglais. longueurPath ou lenghtChemin sont des noms pour le moins curieux !  

## À propos des environnements de développement

Vous avez à votre disposition des environnements de développement (IDE). Pensez à les utiliser et apprenez à exploiter leurs nombreuses possibilités.

La plupart de ces environnements vous offrent des outils de refactoring qui vous permettent de réorganiser votre code facilement tout en garantissant une certaine cohérence. Par exemple, ils vous permettent de renommer une variable partout dans le code. C'est l'occasion de changer tous vos plop par des noms plus significatifs.

En général, ces outils vous permettent également de vérifier que votre code est correctement indenté, et qu'il respecte des conventions de programmation préétablies et matérialisées par des règles. Vous devez apprendre à les utiliser, cela vous fera gagner beaucoup de temps.

Ces outils vous offrent également des fonctionnalités d'auto-complétion (c'est-à-dire qu'ils complètent automatiquement le texte que vous êtes en train de taper). Ce sont des fonctionnalités très pratiques qu'il faut également apprendre à maîtriser. Grâce à ces fonctionnalités, vous n'avez plus d'excuses : inutile de choisir des noms de variables courts (type a b c) sous prétexte que c'est plus rapide à taper...

### Enfin, Il faut aussi noter que certains languages utilisent des normes specifiques à respecter, par exemple les normes PSR pour le PHP.