# Interrable
A second brain for Claude code

# 🧠 Second Brain — mémoire auto-corrective pour Claude Code

Un cerveau externe, simple, que Claude Code lit et **réécrit lui-même** au fil
des sessions — pas juste pour se souvenir de toi, mais pour affiner sa propre
façon de travailler avec toi, et corriger ses règles quand elles ne marchent
plus.

## Ce qui rend ce cerveau différent

La plupart des systèmes de mémoire stockent des **faits** ("l'utilisateur
préfère X"). Celui-ci stocke des **règles de comportement versionnées**
("je dois faire X") que Claude remplace lui-même quand elles s'avèrent
fausses — sans les dupliquer, sans les laisser s'accumuler en silence.

Exemple concret :
- Session 1 : Claude se note "toujours proposer 3 options avant de coder"
- Session 5 : l'utilisateur dit "non, vas-y direct"
- Claude **remplace** la règle au lieu d'en garder deux qui se contredisent

## Tu n'as jamais utilisé de terminal ? Lis ça d'abord

Claude Code (le produit, différent de claude.ai) se lance dans un **terminal**
— une fenêtre où on tape des commandes texte au lieu de cliquer. C'est normal
et volontaire : Claude Code doit pouvoir lire/écrire des fichiers et exécuter
des commandes sur ta machine, ce qu'une page web ne permet pas.

- **Mac :** Cmd+Espace, tape "Terminal", Entrée
- **Windows :** cherche "Terminal" dans le menu démarrer (ou utilise WSL)
- **Linux :** déjà familier normalement

## Installation (une seule fois)

```bash
# 1. Télécharge/clone ce dossier où tu veux sur ton ordinateur
git clone <url-de-ton-repo> second-brain
cd second-brain

# 2. Rends les hooks exécutables
chmod +x .claude/hooks/*.sh

# 3. Lance Claude Code depuis ce dossier
claude
