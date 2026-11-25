---
name: "preparer-clear"
description: "Quand l'utilisateur écrit /clear, « clear » ou « on repart à zéro » dans n'importe quelle conversation : tout sauvegarder dans un fichier d'état pour pouvoir reprendre après une remise à zéro."
---

# Préparer une remise à zéro (/clear)

Claude ne peut pas vider la conversation lui-même : seul l'utilisateur peut taper la commande /clear. Ce skill garantit qu'après /clear, rien d'utile n'est perdu et qu'une nouvelle conversation peut reprendre le travail.

Valable pour toutes les conversations (code, commercial, site web, réseaux, dossiers, etc.).

## Étapes

1. Identifier la liste de suivi de la conversation (liste datée, état, plan) dans le projet ou le dépôt. S'il n'y en a pas, en créer une : `etat-<sujet>.md`.
2. Y écrire un état de reprise complet et autonome :
   - **Règles et consignes** données par l'utilisateur (toutes, y compris « ne pas faire »).
   - **État actuel** : ce qui est fait, livré, programmé, en cours, avec liens, identifiants et chemins utiles (fichiers, branches, campagnes, documents).
   - **Actions datées restantes**, du plus proche au plus lointain.
   - **En attente** : réponses, validations.
   - **Comment reprendre** : la phrase à dire dans une nouvelle conversation (ex. « lis etat-<sujet>.md puis fais ce que tu as à faire »).
3. Archiver l'ancienne version si le fichier existait (copie datée), puis enregistrer la nouvelle.
4. Relire le fichier écrit et vérifier qu'aucune consigne ni échéance n'a disparu.
5. Répondre en trois lignes : où l'état est sauvegardé, la phrase de reprise, puis « Tu peux taper /clear. »

## Règles

- Aucune action externe (envoi, publication, suppression) pendant ce skill.
- Ne jamais résumer une consigne au point d'en changer le sens.
- Phrases courtes, dans la langue de l'utilisateur.
