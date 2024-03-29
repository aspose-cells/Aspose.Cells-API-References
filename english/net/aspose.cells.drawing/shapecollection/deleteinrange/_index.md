---
title: ShapeCollection.DeleteInRange
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Delete shapes in the range.Comment shapes will not be deleted
type: docs
url: /net/aspose.cells.drawing/shapecollection/deleteinrange/
---
## ShapeCollection.DeleteInRange method

Delete shapes in the range.Comment shapes will not be deleted.

```csharp
public void DeleteInRange(CellArea ca)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range.If the shapes are contained in the range, they will be removed. |

### Examples

```csharp

[C#]
//add first shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//add second shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

CellArea area3 = new CellArea();
area3.StartColumn = 0;
area3.StartRow = 5;
area3.EndColumn = 5;
area3.EndRow = 8;

//del
shapes.DeleteInRange(area3);
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


