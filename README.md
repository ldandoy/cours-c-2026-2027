La demande du client
Votre cliente, Martine, vous a laissé ce message vocal. Votre mission : lui livrer le programme qu'elle décrit. Lisez-le en entier avant d'écrire quoi que ce soit.

« Bonjour ! Moi c'est Martine, je loue des kayaks sur la Marne. Aujourd'hui je fais tout sur un carnet et je me trompe sans arrêt dans les prix, alors je voudrais un petit programme pour l'ordinateur de l'accueil.

Les gens arrivent, ils me disent combien ils sont et combien de temps ils veulent partir, et moi je veux savoir combien leur faire payer. C'est 12 € par personne pour une heure, 20 € la demi-journée et 32 € la journée complète. Les enfants de moins de 12 ans paient moitié prix. Par contre, ils ne partent jamais sans un adulte : ça, c'est mon assurance qui l'exige.

Le week-end, c'est 2 € de plus par personne, c'est mon mari qui a voulu ça. Pour un groupe de 10 personnes ou plus, je fais 10 % sur le total. Les gilets sont compris, il faut le dire aux gens.

Ah, et je prends une caution de 50 € par kayak, que je rends au retour. Ça ne compte pas dans le prix, mais il faut que je sache combien encaisser. Mes kayaks sont tous des biplaces.

Mon neveu m'a dit que ce n'était pas compliqué à faire. »

Règle du jeu : votre professeur joue le rôle de Martine. S'il vous manque une information, allez lui poser la question. Elle ne répond qu'aux questions qu'on lui pose.

## Les variables du programme

Voici les variables dont votre programme a besoin. Pour chacune, retrouvez dans le message de Martine la phrase qui la justifie.

**Ce que l'on demande à l'accueil (saisies) :**

| Nom | Type | Ce qu'elle contient | Exemple |
| --- | --- | --- | --- |
| `nb_adultes` | `int` | Nombre d'adultes dans le groupe | 2 |
| `nb_enfants` | `int` | Nombre d'enfants de moins de 12 ans | 1 |
| `duree` | `int` | Durée choisie : 1 = une heure, 2 = demi-journée, 3 = journée | 2 |
| `week_end` | `int` | 1 si c'est le week-end, 0 sinon | 0 |

**Ce que le programme calcule :**

| Nom | Type | Ce qu'elle contient | Exemple |
| --- | --- | --- | --- |
| `nb_personnes` | `int` | Adultes et enfants ensemble | 3 |
| `prix_adulte` | `float` | Prix pour un adulte, selon la durée et le jour | 20.00 |
| `prix_enfant` | `float` | Prix pour un enfant, selon la durée et le jour | 10.00 |
| `prix_total` | `float` | Prix de la location pour tout le groupe, remise comprise | 50.00 |
| `nb_kayaks` | `int` | Nombre de kayaks biplaces nécessaires | 2 |
| `caution` | `int` | Caution à encaisser pour tous les kayaks | 100 |
| `total_encaisse` | `float` | Ce que Martine encaisse : prix et caution | 150.00 |

Question à vous poser : pourquoi `prix_total` est-il un `float` alors que tous les tarifs de Martine sont des nombres entiers ?

## Étape 1 — Les actions, sur une feuille

Avant de toucher au clavier, écrivez sur papier, en français, toutes les actions que le programme doit faire, dans l'ordre. Faites valider votre feuille par le professeur avant de passer au code.

**Règles d'écriture :**

- une seule action par ligne, et des lignes numérotées ;
- chaque ligne commence par un verbe : *Demander*, *Lire*, *Calculer*, *Si … alors*, *Sinon*, *Afficher* ;
- utilisez les noms de variables du tableau ci-dessus ;
- écrivez les conditions en entier : « Si `duree` vaut 1 alors … ».

Exemple pour démarrer :

```
1. Afficher "Nombre d'adultes : "
2. Lire nb_adultes
3. ...
```

**Avant de rendre votre feuille, vérifiez qu'elle répond à ces questions :**

1. Que se passe-t-il si un groupe arrive avec 2 enfants et aucun adulte ?
2. Combien de kayaks faut-il pour 3 personnes ? Pour 1 personne ?
3. Le samedi, combien paie un enfant pour une heure ?
4. Un groupe de 8 adultes et 4 enfants a-t-il droit à la remise ?

Si vous ne savez pas répondre à l'une d'elles, c'est qu'il vous manque une information : allez interroger Martine.

**Testez votre feuille à la main.** Suivez vos lignes une par une avec le cas « 2 adultes, 1 enfant, demi-journée, en semaine », en notant la valeur de chaque variable. Vous devez trouver un prix de 50 €, 2 kayaks et une caution de 100 €.
