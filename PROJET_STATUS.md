# Projet 2 — Coach LinkedIn Patrimoine

## Statut : en cours
Démarré le 15/05/2026.

## Objectif
Générer des posts LinkedIn/semaine sur la niche patrimoine
en surveillant Google Alerts RSS et YouTube (à venir).

## Stack
- n8n (orchestration, self-hosted WSL2)
- Claude API / Haiku (rédaction posts)
- Gmail (livraison)

## Ce qui est en place
- Repo GitHub créé
- PROJET_STATUS.md branché dans le mail quotidien n8n
- Coach quotidien opérationnel (lit commits + backlog des 2 projets, mail 7h)
- Pipeline hebdomadaire opérationnel (dimanche soir)
  - 3 flux RSS en parallèle (PER individuel, Plan épargne retraite, Assurance vie fiscalité)
  - Filtre pertinence sur les titres
  - Génération posts via Claude Haiku
  - Envoi mail avec source citée
- Workflows n8n exportés et versionnés dans /workflows

## En cours
- Améliorer le ton via few-shot prompting (exemples de posts à rédiger)

## Prochaine étape
- [ ] Écrire 3 posts exemples dans mon ton et les injecter dans le prompt
- [ ] Brancher YouTube RSS (chaînes finance FR : Heureka, Protheo...)
- [ ] Tester avec plusieurs items filtrés en même temps


## Coût estimé
~0,05$/run hebdomadaire avec Claude Haiku + prompt court