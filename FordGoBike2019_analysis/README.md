# Ford Gobike - exploration du jeu de données de Février 2019
## par Lamine Bellilet


## Dataset


Le jeu de données comporte 183412 trajets enregistrés, avec 16 données différents sur ces dernier dont la durée, les heures et stations de départ et d'arrêt, l'âge et le sexe des utilisateurs et leurs status vis-à-vis le système Gobike et Bike share for all.
Il y a des données manquantes notamment sur les stations, l'année de naissance des utilisateurs et leur sexe. Ce manque représente un nombre négligeable relativement au volume du jeu, donc ils sont supprimés dans le tableau sur lequel l'analyse est effectuée. De faux types de données et des données aberrantes sont aussi à noter. Le premier issu est corrigé adéquatement en corrigeant les types. Quant aux données aberrantes, elles sont exclues là ou elles posent problème.

Pour une analyse plus riche, de nouvelles variables sont créer, à noter :
- l'âge (à partir de l'année de naissances des utilisateurs),
- l'heure de départ et le jour de semaine (à parti de l'heure exacte de départ),
- la durée en minutes du trajet (à parti de la durée en seconde).


## Summary of Findings

L'analyse exploratoire est effectuée sur toutes les variables d'intérêt, en tenant compte des outliers qui se présente au fur et à mesure notamment au niveau de l'âge des utilisateurs et la durée des trajets.

l'analyse univariée a révélé le suivant:
- durée moyenne (min) : les trajets sont majoritrairement autour de 10 min, ce qui est trois fois moins que la première option du service Gobike (30 min),
- abnnements : 90% des utilisateurs sont des abonnés,
- sexe : le système est beaucoup plus sollicité par les hommes (76%) que les femmes (23%),
- programme Bike Share For All : 90% des utilisateurs ne font pas partie de ce programme; il manque leur status social dans le jeu de données, il est donc impossible de conclure qu'il s'agit de résidents à faible revenus qui ignore l'existence du programme.
- âge : en moyenne autour de 30, avec les plus de 40 rivalisant avec les moins de 30 ans,
- heure des trajets : le système connait une forte demande autour des heures de pointes.

l'analyse bivariée et multivariée:
- les trajets augmentent durant les jours de semaine contrairement au weekend ou l'activitée connait un seul pic autour de 15h et la durée moyenne augmente légèrement.
- la durée moyenne des trajets baisse en fonction de l'âge, et ce plus rapidement chez les femmes que chez les hommes qui maintiennent une durée relativement longue même après 40 ans.
- les autres variables ne présentent pas un motif récurrent remarquable ou une forte corrélation à signaler.


## Key Insights for Presentation

Le déplacement à vélos diffère selon l'heure et le jour de la semaine. C'est parmi les résultats importants de cette analyse. Ceci est présenté avec des titres des axes plus significatifs et des paramètre favorisant la clareté. J'ai aussi opté pour la présentation adjacente de certains graphes complémentaires de par leur contenus pour en accentuer le sens.