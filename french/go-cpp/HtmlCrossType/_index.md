---
title: "Enum HtmlCrossType"
linktitle: "HtmlCrossType"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Enum HtmlCrossType. Encapsule l'objet qui représente htmlcrosstype en Go."
type: docs
weight: 200
url: /fr/go-cpp/htmlcrosstype/
---

## HtmlCrossType Enum

Représente cinq types de chaîne croisée HTML.

```go

type HtmlCrossType int32


```

## Champs

| Champ | Description |
| --- | --- |
| [Default](./default/) | Affiche comme MS Excel, dépend de la cellule suivante. Si la cellule suivante est nulle, la chaîne traversera, ou sera tronquée. |
| [MSExport](./msexport/) | Affiche la chaîne comme MS Excel lors de l'exportation HTML. |
| [Cross](./cross/) | Affiche la chaîne HTML croisée, cette performance pour créer de gros fichiers html sera plus de dix fois plus rapide que de définir la valeur sur Default ou FitToCell. |
| [CrossHideRight](./crosshideright/) | Affiche la chaîne HTML croisée et masque la chaîne de droite lorsque les textes se chevauchent. |
| [FitToCell](./fittocell/) | Affiche uniquement la chaîne à l'intérieur de la largeur de la cellule. |
