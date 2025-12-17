# Feature: Security Audit Agent

## Contexte
Pour garantir la fiabilité du code produit par le Builder, nous avons besoin d'un agent tiers de vérification.

## Objectif
Ajouter un agent "Auditor" (GLM 4.6) dans la configuration `openspec/agents.yaml`.

## Spécifications Techniques
L'agent doit être configuré ainsi :
1. **Auditor** :
   - Role: Security Guard
   - Mission: Analyser chaque PR/Commit pour détecter les failles.
   - Tools: Read-only access to file system.
   - Constraints:
     - Bloquer tout code qui exécute des commandes système non autorisées.
     - Vérifier l'absence de secrets (clés API) en dur.
