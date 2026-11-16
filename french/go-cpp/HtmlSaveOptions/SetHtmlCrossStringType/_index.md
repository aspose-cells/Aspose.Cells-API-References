---
title: "SetHtmlCrossStringType Méthode"
linktitle: "SetHtmlCrossStringType"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "SetHtmlCrossStringType méthode. Encapsule la fonction qui représente sethtmlcrossstringtype en Go."
type: docs
weight: 200
url: /fr/go-cpp/htmlsaveoptions/sethtmlcrossstringtype/
---

## SetHtmlCrossStringType function

Indique si une chaîne s'étendant sur plusieurs cellules sera affichée de la même manière que MS Excel lors de l'enregistrement d'un fichier Excel au format HTML. Par défaut, la valeur est Default, ainsi, pour les chaînes multi‑cellules, il y a peu de différence entre les fichiers HTML créés par Aspose.Cells et MS Excel. Mais les performances pour créer de gros fichiers HTML, en définissant la valeur à Cross, seraient plusieurs fois plus rapides que de la définir à Default ou Fit2Cell.

```go

func (instance *HtmlSaveOptions) SetHtmlCrossStringType(value HtmlCrossType)  error

```

## Remarques


## Voir aussi

* Class [HtmlSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
