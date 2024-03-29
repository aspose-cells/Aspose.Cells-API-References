---
title: AddLabel
second_title: Référence de l'API Aspose.Cells pour .NET
description: Ajoute une étiquette à la feuille de calcul.
type: docs
weight: 130
url: /fr/net/aspose.cells.drawing/shapecollection/addlabel/
---
## ShapeCollection.AddLabel method

Ajoute une étiquette à la feuille de calcul.

```csharp
public Label AddLabel(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| upperLeftRow | Int32 | Index de ligne en haut à gauche. |
| top | Int32 | Représente le décalage vertical de Label par rapport à sa ligne de gauche, en pixels. |
| upperLeftColumn | Int32 | Index de la colonne en haut à gauche. |
| left | Int32 | Représente le décalage horizontal de Label par rapport à sa colonne de gauche, en pixels. |
| height | Int32 | Représente la hauteur de Label, en unité de pixel. |
| width | Int32 | Représente la largeur de Label, en unité de pixel. |

### Return_Value

Un objet Étiquette.

### Exemples

```csharp

[C#]
// ajouter une étiquette
Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
```

### Voir également

* class [Label](../../label)
* class [ShapeCollection](../../shapecollection)
* espace de noms [Aspose.Cells.Drawing](../../shapecollection)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
