---
title: "ShapeCollection.AddCopy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute et copie une forme dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addcopy/
---
## AddCopy(Shape, int, int, int, int) {#addcopy}

Ajoute et copie une forme à la feuille de calcul.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceShape | Forme | Forme source. |
| topRow | Int32 | L'index de la ligne supérieure. |
| haut | Int32 | Représente le décalage vertical depuis sa ligne supérieure, en unité de pixel. |
| leftColumn | Int32 | L'index de la colonne de gauche. |
| gauche | Int32 | Représente le décalage horizontal depuis sa colonne de gauche, en unité de pixel. |

### Valeur de retour

Le nouvel objet [`Shape`](../../shape/).

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCopyWithShapeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;

            // Ajouter une forme rectangulaire
            RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Ajouter une copie de la forme rectangle avec une nouvelle position
            shapes.AddCopy(rectangle, 7, 0, 7, 0);

            // Enregistrez le classeur
            workbook.Save("ShapeCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Shape, int, int, int, int, CopyOptions) {#addcopy_1}

Ajoute et copie une forme à la feuille de calcul.

```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left, 
    CopyOptions copyOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceShape | Forme | Forme source. |
| topRow | Int32 | L'index de la ligne supérieure. |
| haut | Int32 | Représente le décalage vertical depuis sa ligne supérieure, en unité de pixel. |
| leftColumn | Int32 | L'index de la colonne de gauche. |
| gauche | Int32 | Représente le décalage horizontal depuis sa colonne de gauche, en unité de pixel. |
| copyOptions | CopyOptions | Les options de copie des formes. |

### Valeur de retour

Le nouvel objet [`Shape`](../../shape/).

### Exemples

```csharp

[C#]
//ajouter une forme
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//Ajoute et copie une forme.
shapes.AddCopy(rectangle, 7, 0, 7, 0);
```

### Voir aussi

* class [Shape](../../shape/)
* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


