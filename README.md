<!--
  MODÈLE DE README — Pipeline Data, séquence 1, chapitre 5
  Les blocs comme celui-ci sont des consignes : GitHub ne les affiche pas.
  Remplace chaque [crochet] par ton texte, puis supprime les crochets.
  Repères Markdown : une ligne qui commence par # est un titre ; une ligne qui commence par - est une puce.
-->

# Projet Final : Anticiper la montée en charge des réseaux mobiles. 

<!-- Une phrase qui dit ce que fait ton projet. Exemple : « Prévoir la production de 6 boulangeries selon la météo pour réduire les invendus. » -->
Prédire l'évolution du trafic national de données mobiles et identifier les territoires présentant une pression potentielle sur les infrastructures radiomobiles en France métropolitaine, afin d'orienter la planification du déploiement des antennes.

## 1. Le problème

<!-- Reprends ta fiche projet : le contexte en 2 ou 3 phrases, la question centrale, l'utilisateur. -->
- **Contexte** : L’augmentation de la consommation des données mobiles et le développement des réseaux mobiles 4G et 5G posent de nouveaux enjeux aux opérateurs télécoms en matière de dimensionnement et de planification de déploiement des antennes.
- **Question centrale** : Comment prédire l'évolution du trafic national de données mobiles et identifier les territoires présentant une pression potentielle sur les infrastructures radiomobiles en France métropolitaine, afin d'orienter la planification du déploiement des antennes ?
- **Utilisateur** : Opérateurs Télécoms

## 2. Les données

<!-- Une ligne par source envisagée, comme dans ta fiche projet. -->
| Source | Type | Ce qu'elle apporte |
| --- | --- | --- |
| Données sur les réseaux mobiles, ANFR | API | Localiser les stations mobiles (sites 4G/5G), identifier les opérateurs, les technologies déployées avec les coordonnées géographiques, commune, département, la date de mise en service, le statut technique (en service, projet approuvé,...) |
| Qualité de service mobile, ARCEP | CSV | La qualité de service (QoS) à travers le débit descendant, débit montant, signal radio pour chaque opérateur avec la localisation, commune. |
| Observatoire des communications électroniques, ARCEP | Excel| L’historique du volume de données mobiles consommés. |
| Population par commune, INSEE | Excel| La population communale, avec les identifiants département et région. |
| Contours géographiques – IGN, DATA.GOUV | GEOJson | Les données géographiques et administratives sur les communes : commune, la géométrie : un polygone (ensemble de coordonnées GPS délimitant le contour de la commune), département, région. |

## 3. L'organisation du dépôt

<!-- Laisse cette liste telle quelle : elle décrit les dossiers créés au chapitre 3. -->
- `data/raw/` : les données brutes, telles que reçues, jamais modifiées
- `data/processed/` : les données nettoyées, prêtes pour l'analyse
- `notebooks/` : les notebooks Jupyter d'exploration et d'analyse
- `scripts/` : les scripts Python du projet
- `sql/` : les requêtes SQL
- `api/` : l'API du projet
- `dashboard/` : le rapport Power BI et ses captures d'écran
- `docs/` : la fiche projet et les documents du projet

## 4. L'avancement

<!-- Les étapes de ton projet. La première est faite. Tu cocheras les suivantes une fois le module terminé, quand tu appliqueras chaque méthode à ton projet : remplace alors [ ] par [x]. -->
- [x] Sujet choisi, dossiers créés, dépôt publié
- [ ] Collecte des données
- [ ] Requêtes SQL
- [ ] Nettoyage et dataset final
- [ ] Stockage en base
- [ ] API
- [ ] Analyse et tableau de bord

---
Mamadou Diallo· Formation Data Analyst & IA · DataSuits
