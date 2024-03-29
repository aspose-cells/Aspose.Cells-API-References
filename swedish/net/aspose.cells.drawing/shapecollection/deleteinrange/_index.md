---
title: DeleteInRange
second_title: Aspose.Cells för .NET API-referens
description: Ta bort former i intervallet. Kommentarsformer kommer inte att tas bort.
type: docs
weight: 390
url: /sv/net/aspose.cells.drawing/shapecollection/deleteinrange/
---
## ShapeCollection.DeleteInRange method

Ta bort former i intervallet. Kommentarsformer kommer inte att tas bort.

```csharp
public void DeleteInRange(CellArea ca)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | CellArea | Omfånget. Om formerna finns i intervallet kommer de att tas bort. |

### Exempel

```csharp

[C#]
//lägg till första formen
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//lägg till en andra form
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

CellArea area3 = new CellArea();
area3.StartColumn = 0;
area3.StartRow = 5;
area3.EndColumn = 5;
area3.EndRow = 8;

//del
shapes.DeleteInRange(area3);
```

### Se även

* struct [CellArea](../../../aspose.cells/cellarea)
* class [ShapeCollection](../../shapecollection)
* namnutrymme [Aspose.Cells.Drawing](../../shapecollection)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
