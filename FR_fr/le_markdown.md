# Initiation au langage Markdown

## Introduction

Le langage markdown est un langage de formatage de documents (il n'est donc pas un langage de programmation à proprement parler), c'est un langage de balisage (comme le HTML, le LaTeX, etc..) aux fonctionnalités limitées mais groupant les essentielles pour créer de la documentation formatée en ligne.

Pour créer du markdown un simple éditeur de texte brut suffit (le bloc-notes windows suffit donc) même si des outils plus spécialisés ont vu le jour (et plus intuitifs) ce qui sera abordé par la suite.

## Le principe

Le principe de ce langage est l'utilisation de caractères comme balise, les logiciels capables d'afficher du markdown interprètent ces balises et formatent la partie du document balisée en conséquence.

## Pourquoi ce langage ?

Ce langage 

## Où trouve-t-on ce langage ?

Ce langage s'utilise beaucoup dans la communauté des développeurs qui utilisent des systèmes de versionnage de fichiers ou de travaux collaboratifs. Tous les utilisateurs et utilisatrices de « git » l'ont déjà vu s'ils ne le pratiquent pas.

## Les balisages textuels

Je range le balisage textuel dans 2 catégories : le formatage textuel et la structure documentale. 

### Le balisage textuel

Avant de les traiter je repose ici quelques concepts relatifs à la mise en valeur d'un texte. Le texte est simple comme celui-ci, mais *il peut être en emphase légère comme celui-ci* ou bien **il peut être en emphase forte, comme celui-là**. Par habitude (mauvaise ?) on associe l'emphase légère à l'*italique* et l'emphase forte au **gras**.

Pour que les symboles * et _ soient intérprétés comme des balises et non des caractères à afficher naturellement, le symbole doit être collé à la première lettre de la partie à formater et à la dernière lettre. Ainsi `* bonjour *` affiche * bonjour * alors que `*bonjour*` affiche *bonjour*.

#### L'emphase légère

L'emphase légère se fait en entourant avec * ou avec _ le bloc de texte ou le mot qui doit être mis en valeur. Attention : le symbole doit toucher la première et le symbole la dernière.

Ainsi `*bonjour*` et `_bonjour_` donneront *bonjour* et _bonjour_. Vous voyez une différence ? Aucune pas vrai ?

La même chose reste valable pour un morceau de phrase ou un paragraphe entier :

```
	*Ceci est un paragraphe en plusieurs lignes qui sera en emphase légère car l'italique c'est bien mais l'emphase c'est mieux. Pour reprendre les propos de Bourvil je dirais que « l'alcool non, mais l'eau ferrugineuse ... »*
```

Ce qui donne :

*Ceci est un paragraphe en plusieurs lignes qui sera en emphase légère car l'italique c'est bien mais l'emphase c'est mieux. Pour reprendre les propos de Bourvil je dirais que « l'alcool non, mais l'eau ferrugineuse ... »*

### Le balisage de la structure documentale.

Vous aurez remarqué que le document affiche des titres, des sous-titre etc... par des polices de caractères plus grandes et en gras (emphase forte), ces titres sont eux-même balisés grâce au symbole #. Vont suivre un extrait de code et son résultat formaté.

	# Titre principal (niveau 1)
	
	## Sous-titre (niveau 2)
	
	### Sous-sous-titre (niveau 3)
	
	#### sous-sous-sous-titre (niveau 4)

Ce qui donne :

# Titre principal (niveau 1)
	
## Sous-titre (niveau 2)
	
### Sous-sous-titre (niveau 3)
	
#### sous-sous-sous-titre (niveau 4)

etc. etc.

## Le balisage de listes

Il existe deux sortes de listes, les listes à puce qui pourront être balisées par les symboles `*` ou `_` et les listes numérotées.

### Les listes à puce

Très pratiques et souvent utilisées, les listes à puce sont simplement des lignes de textes qui seront préfixées par `- ` (tiret et espace) ou bien par `* ` (étoile et espace). Ainsi le code suivant :

	* ceci est la première ligne de la liste
	* ceci est la 2nde ligne du code
	* Voici la 3e

donnera :

* ceci est la première ligne de la liste
* ceci est la 2nde ligne du code
* Voici la 3e

La même chose s'obtient avec le symbole `-` :

	- ceci est la première ligne (bis)
	- ceci est la seconde ligne de code
	- et ceci la 3e

donnera :

- ceci est la première ligne (bis)
- ceci est la seconde ligne de code
- et ceci la 3e

#### Cas des listes imbriquées.

Les listes peuvent être imbriquées les unes dans les autres, il suffit alors de tabuler avant le symbole choisi `-` ou `*`

- niveau 1, ligne 1
- niveau 1, ligne 2
- niveau 1, ligne 3
	- niveau 2, ligne 1
	- niveau 2, ligne 2
	- niveau 3, ligne 3
- niveau 1, ligne 4

## Les balisages de tableaux

## Les balisages de liens

## Les balisages d'images

## Les balisages de code

## Les extensions : le balisage de formules LaTeX
