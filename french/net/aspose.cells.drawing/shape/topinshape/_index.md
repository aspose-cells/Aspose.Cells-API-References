---
title: "Shape.TopInShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente le décalage vertical de la forme par rapport à la bordure supérieure de la forme parente, en unité de 1/4000 de la hauteur de la forme parente"
type: docs
url: /fr/net/aspose.cells.drawing/shape/topinshape/
---
## Shape.TopInShape property

Représente le décalage vertical de la forme par rapport à la bordure supérieure de la forme parent, en unité de 1/4000 de la hauteur de la forme parent.

```csharp
public int TopInShape { get; set; }
```

### Remarques

S'applique uniquement lorsque cette forme se trouve dans le groupe ou le graphique.

### Exemples

```csharp

[C#]
if (shape.IsInGroup && shape.TopInShape == 8000)
    shape.TopInShape = 4000;
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


