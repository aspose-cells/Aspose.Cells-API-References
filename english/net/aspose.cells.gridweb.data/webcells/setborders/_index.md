---
title: WebCells.SetBorders
second_title: Aspose.Cells for .NET API Reference
description: WebCells method. Sets borders for a cells range
type: docs
url: /net/aspose.cells.gridweb.data/webcells/setborders/
---
## WebCells.SetBorders method

Sets borders for a cells range.

```csharp
public void SetBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, 
    SetBorderPosition position, WebBorderStyle borderStyle)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The first row number of the range(zero based). |
| firstColumn | Int32 | The first column number of the range(zero based). |
| rowNumber | Int32 | The rows number. |
| columnNumber | Int32 | The columns number. |
| position | SetBorderPosition | The border position. |
| borderStyle | WebBorderStyle | The border style. |

### Examples

```csharp
[C#]
	GridWeb1.WebWorksheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### See Also

* enum [SetBorderPosition](../../../aspose.cells.gridweb/setborderposition/)
* class [WebBorderStyle](../../../aspose.cells.gridweb/webborderstyle/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


