# Arbre local

Moteur de recherche généalogique 100 % local sur les 29 millions de décès enregistrés en France depuis 1970. La recherche s'exécute entièrement dans le navigateur (DuckDB-WASM + Parquet + HTTP Range Requests) : aucun nom saisi n'est envoyé à un serveur.

**Site : https://xensma.github.io/arbre-local/**

Basé sur le tutoriel [sosoj92/arbre-local](https://github.com/sosoj92/arbre-local).

## Sources et licences

- Fichier des personnes décédées — INSEE / data.gouv.fr, Licence Ouverte 2.0 (téléchargé le 09/08/2026). Les lignes marquées `opposition = true` sont exclues, conformément à l'obligation légale.
- Annuaire des services d'archives — Ministère de la Culture / FranceArchives, Licence Ouverte 2.0.

29 305 897 lignes après filtrage (oppositions et dates de naissance invalides écartées), triées par nom et partitionnées par première lettre dans `parts/`.
