# Rétroaction automatisée -- S01 (Diagnostic fondamental -- NexaMart kickoff)

_Générée le 2026-05-15T12:41:59+00:00 -- Run `20260515T122624Z-00a5a04f`_

Ce document est produit par un pipeline reproductible (vérification SQL déterministe + analyse LLM du brief et de la déclaration IA). Une revue humaine précède toujours sa publication. **À ce stade expérimental, aucune note ni étiquette de niveau n'est diffusée : l'objectif est purement formatif.**

> ⚠️ **Avertissement instructeur (à retirer avant publication) :** cette analyse a été générée avec `--skip-pull`. Le contenu correspond au commit local et **n'est peut-être pas la dernière version poussée par l'étudiant·e**.

---

## 1. Vérification automatique de la requête SQL

La requête extraite de votre brief n'a pas pu être validée automatiquement. Quelques pistes constructives ci-dessous pour vous aider à la rendre exécutable et alignee avec la question posée.

_Observation technique : aucun bloc SQL fencé trouvé et extraction LLM échouée_


**Pistes :**
> Aucun bloc ```sql ... ``` détecté. Encadrez votre requête finale dans la section « Preuve » pour fiabiliser l'auto-validation.
> Extracteur LLM : Le brief fourni ne contient aucune requête SQL dans la section 'Preuve' ni ailleurs ; rien à extraire.

## 2. Rétroaction pédagogique sur le brief

> Le brief rendu est essentiellement vide et ne répond pas à la question CEO. Remplissez les sections clés (réponse exécutive, modèle, preuve et validations) en suivant les consignes de format et les contrôles attendus.

### Observations par dimension

**Model quality**
- Observation : brief absent ou trop court
- Piste d'amélioration : Rédiger le schéma de modèle en précisant le grain, les dimensions et mesures, et expliquer comment il répond à la question CEO (150–300 mots au total).

**Validation quality**
- Observation : brief absent ou trop court
- Piste d'amélioration : Fournir au moins une requête SQL de validation qui retourne le résultat attendu et documenter les contrôles (NULLs, doublons, checks de grain).

**Executive justification**
- Observation : brief absent ou trop court
- Piste d'amélioration : Écrire une réponse exécutive en langage décisionnel (150–300 mots) qui indique la recommandation au CEO basée sur les résultats du modèle.

**Process trace**
- Observation : brief absent ou trop court
- Piste d'amélioration : Ajouter un journal de commits (≥3) et une note IA précisant les outils utilisés et la validation humaine pour documenter le processus.

**Reproducibility**
- Observation : brief absent ou trop court
- Piste d'amélioration : Inclure un README et un script 'make check' exécutable permettant à un pair de cloner le dépôt et reproduire les contrôles en <5 minutes.

## 3. Déclaration d'utilisation de l'IA

> La déclaration suit le format attendu et donne un exemple concret de modèle, prompt et validation humaine. Il manque toutefois une mention des limites ou des erreurs observées ; ajoutez une ligne décrivant les limites rencontrées pour chaque interaction.

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

- **Run ID :** `20260515T122624Z-00a5a04f`
- **Devoir :** `S01`
- **Étudiant·e :** `tatanao`
- **Commit analysé :** `6956cc7`
- **Audit (côté instructeur) :** `tools/instructor/feedback_pipeline/audit/20260515T122624Z-00a5a04f/tatanao/`
- **Prompts (SHA-256) :**
  - `sql_extractor_system` : `90ee9e277de7a27f...`
  - `rubric_grader_system` : `505f32d1d8319d66...`
  - `ai_usage_grader_system` : `81cb7fdf89bda55a...`
- **Fournisseur (rubrique) :** `openai`
- **Fournisseur (IA-usage) :** `openai` (gpt-5-mini-2025-08-07)

_Ce feedback a été produit par un pipeline automatisé et **revu par l'équipe pédagogique avant publication**. Aucun chiffre ni étiquette de niveau n'est diffusé à ce stade expérimental : l'objectif est uniquement formatif. Ouvrez une issue dans ce dépôt pour toute question._
