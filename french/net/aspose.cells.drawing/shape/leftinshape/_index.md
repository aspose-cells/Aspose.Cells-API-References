---
title: "Shape.LeftInShape"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente le décalage horizontal de la forme depuis la bordure gauche de la forme parent en unités de 1/4000 de la largeur de la forme parent"
type: docs
url: /fr/net/aspose.cells.drawing/shape/leftinshape/
---
## Shape.LeftInShape property

Représente le décalage horizontal de la forme par rapport à la bordure gauche de la forme parent, en unité de 1/4000 de la largeur de la forme parent.

```csharp
public int LeftInShape { get; set; }
```

### Remarques

S'applique uniquement lorsque cette forme se trouve dans le groupe ou le graphique.

### Exemples

```csharp

[C#]
if (shape.IsInGroup && shape.LeftInShape == 2000)
    shape.LeftInShape = 4000;
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


