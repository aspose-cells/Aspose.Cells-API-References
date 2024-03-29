---
title: CopyInRange
second_title: Aspose.Cells für .NET-API-Referenz
description: Shapes im Bereich in den Zielbereich kopieren.
type: docs
weight: 380
url: /de/net/aspose.cells.drawing/shapecollection/copyinrange/
---
## ShapeCollection.CopyInRange method

Shapes im Bereich in den Zielbereich kopieren.

```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, 
    bool isContained)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceShapes | ShapeCollection | Quellformen. |
| ca | CellArea | Der Quellbereich. |
| destRow | Int32 | Der Zielzeilenindex des Zielbereichs. |
| destColumn | Int32 | Die Zielspalte des Zielbereichs. |
| isContained | Boolean | Ob nur die Formen kopiert werden, die im Bereich enthalten sind. Wenn wahr, werden nur die Formen im Bereich kopiert. Ansonsten funktioniert es wie MS Office. |

### Beispiele

```csharp

[C#]
// eine Form hinzufügen
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
CellArea area2 = new CellArea();
area2.StartColumn = 1;
area2.StartRow = 1;
area2.EndColumn = 5;
area2.EndRow = 11;

//Kopieren
shapes.CopyInRange(shapes, area2, 12, 1, false);

```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea)
* class [ShapeCollection](../../shapecollection)
* namensraum [Aspose.Cells.Drawing](../../shapecollection)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
