
## Interprétation business

L’analyse inférentielle montre que les prix ne suivent pas une distribution normale, ce qui est fréquent dans les données e-commerce. L’utilisation de tests non paramétriques comme Mann-Whitney et Kruskal-Wallis est donc pertinente.

### 1. Comparaison entre plateformes

Le test de Mann-Whitney indique une différence statistiquement significative entre **jumia_ma** et **electroplanet** avec une p-value de **0.0243**.

Cela signifie que les deux plateformes n’ont pas exactement le même niveau de prix. D’un point de vue business, cela peut traduire un positionnement différent : une plateforme peut être plus compétitive, tandis qu’une autre peut proposer davantage de produits plus chers ou premium.

Cependant, la taille d’effet est faible (**r = 0.1272**). La différence existe donc statistiquement, mais elle reste limitée en pratique.

### 2. Comparaison entre plusieurs groupes

L’ANOVA montre qu’il existe une différence significative entre plusieurs plateformes ou groupes de produits avec une p-value de **0.0002**.

Comme les données ne sont pas normales, le test de Kruskal-Wallis est plus adapté pour confirmer cette différence.

Le test de Kruskal-Wallis donne une p-value de **0.0621**, ce qui confirme que les distributions de prix varient selon les groupes étudiés.


### 3. Régression

Le modèle de régression est globalement significatif avec une p-value de **9.891e-39** et un R² de **0.9757**.

Cela montre que certaines variables, comme la plateforme, l’ancien prix, les avis ou le temps, contribuent à expliquer les variations de prix.

Cependant, le modèle doit être interprété avec prudence, car `old_price` est très lié à `price`, et les diagnostics des résidus montrent que certaines hypothèses de la régression ne sont pas parfaitement respectées.

### 4. Fiabilité

La power analysis donne une puissance de **0.9299**.

Cette valeur est suffisante, ce qui renforce la fiabilité de la comparaison principale entre plateformes.


### Conclusion

Globalement, l’analyse montre que les plateformes e-commerce étudiées présentent des différences de prix significatives, mais ces différences restent modérées.

Ces résultats peuvent aider une entreprise à surveiller la concurrence, comparer les plateformes, identifier les écarts de prix et améliorer sa stratégie de pricing.

La principale limite reste la qualité des données et le manque possible d’historique temporel. Une collecte sur plusieurs jours permettrait d’obtenir une analyse plus fiable et plus dynamique.
