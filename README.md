# Moteur de mondes causaux : composer des systèmes complexes dans une boucle commune

[English edition — separate repository](https://github.com/Gaaboy/causal-worlds-engine-public).

Documentation publique d’un projet propriétaire de mondes interactifs (dossier **v1.1**, complété par une note de portée **v1.1.3** · 24 novembre 2026).

**Dossier v1.1 · note complémentaire v1.1.3 · 24 novembre 2026**
Projet mené en solo depuis aout 2024, de la grammaire théorique au runtime expérimental. Développé en vibe coding sur une machine équipée de 8 Go de RAM. Le moteur et ses recettes restent privés. Ce dépôt présente uniquement l’architecture, les résultats de haut niveau et les limites observées.

**Auteur et créateur du projet : Gaaboy.**


> **En 30 secondes** — Cadre théorique états–relations–dynamiques, moteur causal expérimental multi-domaines, instruments de traçabilité et surfaces de création et d’observation. Le dossier couvre les formulations théoriques, l’hystérésis, les identifiants causaux, les points de contrôle, les campagnes intégrées, les calibrations et les limites. Le moteur et ses recettes restent privés; aucun code, configuration ou donnée brute n’est distribué.

## Ce que le projet apporte

Le projet met l’accent sur une boucle expérimentale précise : raccorder des mécanismes spécialisés à un monde commun, suivre la provenance causale déclarée de leurs changements, puis reprendre et comparer des branches pour examiner si une intervention modifie une conséquence ultérieure. Cela donne un cadre concret pour étudier des chaînes comme mémoire → décision → déplacement → ressource, au-delà d’une simple juxtaposition de modules. Un lien d’événement aide à retracer ce que le système consigne; l’attribution causale repose sur les comparaisons et interventions propres au scénario.

Le runtime encadre ses composants par des contrats d’accès et de temps. L’inventaire statique couvre 44 phases et 71 composants : 49 sont classés par pas de référence, 17 par temps écoulé et 5 en régime mixte. Parmi les 32 qui ne reçoivent pas directement `dt`, 2 restent sans dt direct : une projection anatomique à retour différé et une étape de fabrication discrète, qui ne sont pas des taux directs. Trois mécanismes ont maintenant une mise à l’échelle temporelle, selon des hypothèses de taux encore non calibrées; l’un conserve une division discrète à seuil. Le classement organise leur exécution sans prétendre que toutes les cadences ou unités sont déjà harmonisées.

La portée actuelle reste celle des mécanismes et scénarios intégrés et qualifiés. Le dossier ne revendique ni import automatique de tout modèle externe ni validation générale de la grammaire. Les contrats internes, recettes, paramètres détaillés et code demeurent privés.

## Lire le dossier

- **Commencer ici :** [présentation courte en français](Presentation_mondes_interactifs_lite_v1.1.html) · [Markdown](Presentation_mondes_interactifs_lite_v1.1.md)
- [Édition anglaise complète — dépôt séparé](https://github.com/Gaaboy/causal-worlds-engine-public)
- [Dossier technique complet](Presentation_mondes_interactifs_v1.1.md)
- [Dossier complet en HTML](Presentation_mondes_interactifs_v1.1.html)
- [Télécharger le dossier complet en PDF](Presentation_mondes_interactifs_v1.1.pdf)
- [Portée des résultats et priorités de maturation](RESULTS_SCOPE_AND_PRIORITIES.html) · [Markdown](RESULTS_SCOPE_AND_PRIORITIES.md)
- [Page d’accueil visuelle](index.html)
- [Note de portée et de priorités](RESULTS_SCOPE_AND_PRIORITIES.html) · [Markdown](RESULTS_SCOPE_AND_PRIORITIES.md)
- [Notes de publication v1.1.3](RELEASE_NOTES_v1.1.3.md)
- `figures/` — schémas explicatifs du cadre et de ses boucles.

Le dossier technique complet en anglais est publié séparément dans [son propre dépôt GitHub](https://github.com/Gaaboy/causal-worlds-engine-public). Les éditions française et anglaise sont ainsi maintenues dans deux dépôts distincts.

Les PDF conservés dans `archive/v1.0/` appartiennent à l’édition précédente. Le PDF de cette édition v1.1 est disponible ci-dessus et correspond au Markdown et au HTML complets.

## Résultats et mesures observées

### Qualification temporelle en cours

Le dossier décrit la répartition des cadences, les trois mécanismes qui reçoivent une mise à l’échelle par temps écoulé, ainsi que les opérations qui restent discrètes ou à retour différé. La suite ciblée de subdivision, de seuils et de reprise passe **14/14 tests**. Elle qualifie des cas précis : absorption sans division, cible constante pour la cohésion, dynamiques organisationnelles sous support constant et reprise déterministe au pas testé. Les divisions protocellulaires n’ont pas été comparées sous toutes les partitions; les cibles variables, les transitions de support et les coefficients restent à qualifier. Les taux ne sont pas calibrés et aucune synchronisation physique universelle n’est revendiquée.

Le dossier décrit les mécanismes, les campagnes intégrées, les calibrations de domaine, les résultats négatifs et les outils de création et d’observation. Il rapporte notamment une boucle mémoire–trajet–irrigation reproduite dans plusieurs initialisations, des comparaisons de branches collectives, des vérifications ciblées de physique, d’hydrologie, de locomotion, d’optique et de coordination, ainsi qu’un post-mortem de subsistance.

La note [Portée des résultats et priorités de maturation](RESULTS_SCOPE_AND_PRIORITIES.md) synthétise les cinq frontières de lecture — temps, attribution causale, endurance, reproductibilité et généralisation — et les ordonne selon leur lien avec la proposition centrale. Elles encadrent les affirmations; elles ne remplacent pas la description des mécanismes, des campagnes et des fonctions produit.

Les relevés détaillés d’exécution, de ressources et leurs limites sont présentés dans le rapport de campagne ci-dessous.

- [Lire le relevé HTML](evidence/run-record-01/RUN_RECORD.html)
- [Lire le rapport Markdown](evidence/run-record-01/RUN_RECORD.md)
- [Graphique des mesures](evidence/run-record-01/run-metrics.svg)
- [Mesures filtrées à télécharger](evidence/run-record-01/resource-monitor-public.csv)
- [Sorties agrégées à télécharger](evidence/run-record-01/observed-world-output-public.csv)

## Propriété et périmètre

Le projet est propriétaire. Le moteur, le code source et les recettes d’implémentation restent privés. Ce dépôt public ne fournit aucun code source, graine exacte, configuration, commande interne, trace brute, sauvegarde d’exécution, donnée personnelle ou chemin interne. Il s’agit d’un dossier de présentation du projet, pas d’une distribution du moteur.

Les campagnes de tests qui se recouvrent ne sont pas additionnées en un total global. Les résultats rapportés décrivent des scénarios internes précis et leurs limites.

## Droits

© 2026 — Tous droits réservés. Documentation publique fournie à titre informatif. Aucune licence open source n’est accordée sur le moteur, son code source ou ses recettes d’implémentation.

## Archive et citation

Édition française : [Zenodo v1.1.4](https://doi.org/10.5281/zenodo.24538024) · DOI conceptuel (toutes versions) : https://doi.org/10.5281/zenodo.24512314.

