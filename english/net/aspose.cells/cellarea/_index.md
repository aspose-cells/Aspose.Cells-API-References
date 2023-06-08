---
title: Struct CellArea
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CellArea struct. Represent an area of cells
type: docs
url: /net/aspose.cells/cellarea/
---
## CellArea structure

Represent an area of cells.

```csharp
public struct CellArea : IComparable
```

## Methods

| Name | Description |
| --- | --- |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea_1)(string, string) | Creates a cell area. |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea)(int, int, int, int) | Creates a cell area. |
| [CompareTo](../../aspose.cells/cellarea/compareto/)(object) | Compare two CellArea objects according to their top-left corner. |
| override [ToString](../../aspose.cells/cellarea/tostring/)() | Returns a string represents the current cell area object. |

## Fields

| Name | Description |
| --- | --- |
| [EndColumn](../../aspose.cells/cellarea/endcolumn/) | Gets or set the end column of this area. |
| [EndRow](../../aspose.cells/cellarea/endrow/) | Gets or set the end row of this area. |
| [StartColumn](../../aspose.cells/cellarea/startcolumn/) | Gets or set the start column of this area. |
| [StartRow](../../aspose.cells/cellarea/startrow/) | Gets or set the start row of this area. |

### Examples

```csharp

[C#]

//Create Cell Area
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;

[VB.NET]

'Create Cell Area
Dim ca As CellArea = New CellArea()
ca.StartRow = 0
ca.EndRow = 0
ca.StartColumn = 0
ca.EndColumn = 0

```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


