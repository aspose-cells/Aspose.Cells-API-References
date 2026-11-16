---
title: "Classe IconSet"
linktitle: "IconSet"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe IconSet. Encapsule l'objet qui représente iconset en Go."
type: docs
weight: 200
url: /fr/go-cpp/iconset/
---

## IconSet class

Décrit la règle de mise en forme conditionnelle IconSet. Cette règle de mise en forme conditionnelle applique des icônes aux cellules en fonction de leurs valeurs.

```go

type IconSet struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetCfIcons](./getcficons/) | Obtenir theConditionalFormattingIcon de la collection |
| [GetCfvos](./getcfvos/) | Obtenez l'instance de CFValueObjects. |
| [GetType](./gettype/) | Obtenez ou définissez le type de jeu d'icônes à afficher. La définition du type vérifiera automatiquement si le nombre actuel de Cfvos est conforme au nouveau type. Si ce n'est pas le cas, les anciens Cfvos seront nettoyés et les Cfvos par défaut seront ajoutés. |
| [SetType](./settype/) | Obtenez ou définissez le type de jeu d'icônes à afficher. La définition du type vérifiera automatiquement si le nombre actuel de Cfvos est conforme au nouveau type. Si ce n'est pas le cas, les anciens Cfvos seront nettoyés et les Cfvos par défaut seront ajoutés. |
| [IsCustom](./iscustom/) | Indique si le jeu d'icônes est personnalisé. La valeur par défaut est false. |
| [GetShowValue](./getshowvalue/) | Obtenez ou définissez le drapeau indiquant s'il faut afficher les valeurs des cellules sur lesquelles ce jeu d'icônes est appliqué. La valeur par défaut est true. |
| [SetShowValue](./setshowvalue/) | Obtenez ou définissez le drapeau indiquant s'il faut afficher les valeurs des cellules sur lesquelles ce jeu d'icônes est appliqué. La valeur par défaut est true. |
| [GetReverse](./getreverse/) | Obtenez ou définissez le drapeau indiquant s'il faut inverser l'ordre par défaut des icônes dans ce jeu d'icônes. La valeur par défaut est false. |
| [SetReverse](./setreverse/) | Obtenez ou définissez le drapeau indiquant s'il faut inverser l'ordre par défaut des icônes dans ce jeu d'icônes. La valeur par défaut est false. |
