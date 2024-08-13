# `gh pix` GitHub CLI extension

Une extension pour le [GitHub CLI](https://github.com/cli/cli) de basculer sur une branche git du dépôt pix sans connaître son nom, en précisant uniquement le numéro de ticket.

![gh-pix](https://user-images.githubusercontent.com/5627688/133617961-a16d7626-8cab-4e03-9549-7b8892b1e2c5.png)

## Installation
```shell
gh extension install 1024pix/gh-pix
```

### Mise à jour

```shell
gh extension upgrade pix
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

Il est également possible d'entrer le nom du ticket entier (avec le suffixe PIX-) :

```shell
gh pix PIX-1234
```

voire même l'URL Jira du ticket :

```shell
gh pix https://1024pix.atlassian.net/browse/PIX-1234
```

Le script renverra une erreur si la branche n'est pas trouvée (ou si on y est déjà),
et sinon, basculera dessus.
