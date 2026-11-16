---
title: "HyperlinkLoadMode Enum"
linktitle: "HyperlinkLoadMode"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "HyperlinkLoadMode enum. Encapsule l'objet qui représente hyperlinkloadmode en Go."
type: docs
weight: 200
url: /fr/go-cpp/hyperlinkloadmode/
---

## HyperlinkLoadMode Enum

Spécifie comment les hyperliens sont gérés lors du chargement du HTML.

```go

type HyperlinkLoadMode int32


```

## Champs

| Champ | Description |
| --- | --- |
| [Normal](./normal/) | Seul le premier hyperlien d'une cellule est chargé, les suivants sont ignorés. |
| [AllowMultiple](./allowmultiple/) | Tous les hyperliens d'une cellule sont ajoutés à <see cref="Worksheet.Hyperlinks"/>. Notez que MS Excel ne prend en charge qu'un seul hyperlien par cellule, de sorte que cette option peut produire des fichiers que Excel ne peut pas rendre complètement. |
