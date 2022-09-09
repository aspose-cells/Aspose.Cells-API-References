---
title: AddGroupBox
second_title: Référence de l'API Aspose.Cells pour .NET
description: Ajoute un GroupBox à la feuille de calcul.
type: docs
weight: 110
url: /fr/net/aspose.cells.drawing/shapecollection/addgroupbox/
---
## ShapeCollection.AddGroupBox method

Ajoute un GroupBox à la feuille de calcul.

```csharp
public GroupBox AddGroupBox(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| upperLeftRow | Int32 | Index de ligne en haut à gauche. |
| top | Int32 | Représente le décalage vertical de GroupBox par rapport à sa ligne de gauche, en unité de pixel. |
| upperLeftColumn | Int32 | Index de la colonne en haut à gauche. |
| left | Int32 | Représente le décalage horizontal de GroupBox par rapport à sa colonne de gauche, en unité de pixel. |
| height | Int32 | Représente la hauteur de GroupBox, en unité de pixel. |
| width | Int32 | Représente la largeur de GroupBox, en unité de pixel. |

### Return_Value

Un objet GroupBox.

### Exemples

```csharp

[C#]
// ajouter une zone de groupe
GroupBox groupBox = shapes.AddGroupBox(1, 0, 1, 0, 100, 50);
```

### Voir également

* class [GroupBox](../../groupbox)
* class [ShapeCollection](../../shapecollection)
* espace de noms [Aspose.Cells.Drawing](../../shapecollection)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->