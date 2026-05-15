# Rétroaction automatisée -- S01 (Diagnostic fondamental -- NexaMart kickoff)

_Générée le 2026-05-15T12:54:23+00:00 -- Run `20260515T125138Z-ff34aff5`_

Ce document est produit par un pipeline reproductible (vérification SQL déterministe + analyse LLM du brief et de la déclaration IA). Une revue humaine précède toujours sa publication. **À ce stade expérimental, aucune note ni étiquette de niveau n'est diffusée : l'objectif est purement formatif.**

> ⚠️ **Avertissement instructeur (à retirer avant publication) :** cette analyse a été générée avec `--skip-pull`. Le contenu correspond au commit local et **n'est peut-être pas la dernière version poussée par l'étudiant·e**.

---

## 1. Vérification automatique de la requête SQL

La requête extraite de votre brief n'a pas pu être validée automatiquement. Quelques pistes constructives ci-dessous pour vous aider à la rendre exécutable et alignee avec la question posée.

_Observation technique : aucune requête SQL détectée dans le brief_


**Pistes :**
> Aucun bloc ```sql ... ``` détecté et l'extracteur LLM n'a trouvé aucune requête. Encadrez votre requête finale dans la section « Preuve » avec un bloc ```sql ... ``` pour fiabiliser l'auto-validation.
> Extracteur LLM : Le brief fourni ne contient aucune requête SQL dans les sections; aucune requête à extraire.

## 2. Rétroaction pédagogique sur le brief

> Le brief soumis est vide et ne contient aucune des sections attendues ; il est impossible d'évaluer le modèle ou la validation. Remplissez les sections clés (réponse exécutive, modèle, preuve SQL, contrôles) en suivant la structure de l'énoncé pour obtenir des points.

### Observations par dimension

**Model quality**
- Observation : brief absent ou trop court
- Piste d'amélioration : Rédiger le schéma en indiquant le grain (ex. ligne de commande), les dimensions et mesures clés, et justifier les choix de patterns (SCD, bridge, etc.).

**Validation quality**
- Observation : brief absent ou trop court
- Piste d'amélioration : Fournir au moins une requête SQL de validation qui répond à la question CEO et documenter le traitement des cas limites (NULLs, agrégats non-additifs).

**Executive justification**
- Observation : brief absent ou trop court
- Piste d'amélioration : Rédiger un résumé exécutif (150–300 mots) qui répond directement à la question du CEO et propose une recommandation décisionnelle claire.

**Process trace**
- Observation : brief absent ou trop court
- Piste d'amélioration : Ajouter un journal de décisions et lister les commits git (≥3) ou au moins documenter l'usage d'outils IA et la validation humaine réalisée.

**Reproducibility**
- Observation : brief absent ou trop court
- Piste d'amélioration : Inclure un README et un script check (DuckDB) permettant à un collègue de cloner le dépôt et d'exécuter les vérifications sans modification.

## 3. Déclaration d'utilisation de l'IA

> La déclaration contient un exemple utile qui couvre l'outil, l'étape d'utilisation et la validation humaine. Il manque toutefois une mention des limites ou erreurs observées et l'entrée semble être un exemple à remplacer par vos usages réels.

**Sujets bien couverts dans votre déclaration :**

- outils utilisés (nom + version/modèle)
- à quelle étape l'IA a été utilisée
- comment la sortie a été validée par l'humain

**Sujets à ajouter ou expliciter pour la prochaine itération :**

- limites ou erreurs observées

## 4. Pistes d'action pour la prochaine itération

- Reprendre la requête de la section « Preuve » pour qu'elle s'exécute sur `db/nexamart.duckdb` et qu'elle produise la forme attendue (voir pistes en section 1).
- Compléter `ai-usage.md` en y ajoutant : limites ou erreurs observées.

---

## 5. Traçabilité

- **Run ID :** `20260515T125138Z-ff34aff5`
- **Devoir :** `S01`
- **Étudiant·e :** `tatanao`
- **Commit analysé :** `6956cc7`
- **Audit (côté instructeur) :** `tools/instructor/feedback_pipeline/audit/20260515T125138Z-ff34aff5/tatanao/`
- **Prompts (SHA-256) :**
  - `sql_extractor_system` : `90ee9e277de7a27f...`
  - `rubric_grader_system` : `505f32d1d8319d66...`
  - `ai_usage_grader_system` : `81cb7fdf89bda55a...`
- **Fournisseur (rubrique) :** `openai`
- **Fournisseur (IA-usage) :** `openai` (gpt-5-mini-2025-08-07)

_Ce feedback a été produit par un pipeline automatisé et **revu par l'équipe pédagogique avant publication**. Aucun chiffre ni étiquette de niveau n'est diffusé à ce stade expérimental : l'objectif est uniquement formatif. Ouvrez une issue dans ce dépôt pour toute question._
