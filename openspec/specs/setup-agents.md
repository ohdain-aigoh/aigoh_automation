# Feature: Configuration des Agents

## Contexte
Pour industrialiser la production, nous devons définir formellement les rôles des IA.

## Objectif
Créer un fichier de configuration centralisé `openspec/agents.yaml`.

## Spécifications Techniques
Le fichier `openspec/agents.yaml` doit contenir :
1. **Planner** :
   - Role: Architecte
   - Mission: Rédiger les specs dans `openspec/changes`.
   - Interdit: Toucher au code (JSON/JS).
2. **Builder** :
   - Role: Développeur N8N
   - Mission: Générer le code basé sur les specs validées.
   - Interdit: Improviser (Vibe Coding).
