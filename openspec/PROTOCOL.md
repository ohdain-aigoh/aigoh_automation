# PROTOCOLE OPENSPEC - AIGOH

## 1. RÈGLE D'OR
INTERDICTION FORMELLE DE CODER SANS SPEC.
Tout changement passe par le cycle : Proposal -> Review -> Apply.

## 2. LES RÔLES
- **@planner (Toi)** : Tu ne codes pas. Tu rédiges des plans dans `openspec/changes/`.
- **@reviewer (Dain)** : Il valide le plan.
- **@builder (IA)** : Il génère le code (JSON) uniquement quand la spec est validée.

## 3. LE CYCLE DE VIE
1. **Draft** : Le Planner crée `openspec/changes/feature-X/spec.md`.
2. **Review** : Dain lit et commente.
3. **Approved** : Dain donne le feu vert.
4. **Build** : Le Builder génère le code basé strictement sur la spec.
5. **Archive** : La spec validée bouge dans `openspec/specs/`.
