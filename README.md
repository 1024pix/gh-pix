# `gh pix` GitHub CLI extension

Une extension pour le [GitHub CLI](https://github.com/cli/cli) de basculer sur une branche git du dépôt pix sans connaître son nom, en précisant uniquement le numéro de ticket.

## Installation
```shell
gh extension install 1024pix/gh-pix
```

## Usage

Pour basculer sur la branche correspondant au ticket PIX-1234, on écrira :

```shell
gh pix 1234
```

Ce qui équivaut à faire :

```shell
git checkout pix-1234[TAB][ENTRÉE]
```

Soit 14 frappes de touches en moins !

Le script renverra une erreur si la branche n'est pas trouvée (ou si on y est déjà),
et sinon, basculera dessus.
