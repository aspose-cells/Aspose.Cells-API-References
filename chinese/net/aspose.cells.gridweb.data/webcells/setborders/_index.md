---
title: "WebCells.SetBorders"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WebCells 方法。为单元格范围设置边框"
type: docs
url: /zh/net/aspose.cells.gridweb.data/webcells/setborders/
---
## WebCells.SetBorders method

为单元格范围设置边框。

```csharp
public void SetBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, 
    SetBorderPosition position, WebBorderStyle borderStyle)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | Int32 | 范围的第一行编号（从零开始）。 |
| firstColumn | Int32 | 范围的第一列编号（从零开始）。 |
| rowNumber | Int32 | 行数。 |
| columnNumber | Int32 | 列数。 |
| 位置 | SetBorderPosition | 边框位置。 |
| borderStyle | WebBorderStyle | 边框样式。 |

### 示例

```csharp
[C#]
	GridWeb1.WebWorksheets[0].Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1);

[VB]
	GridWeb1.WebWorksheets(0).Cells.SetBorders(0, 0, 5, 8, SetBorderPosition.Outline, borderStyle1)
```

### 另请参见

* enum [SetBorderPosition](../../../aspose.cells.gridweb/setborderposition/)
* class [WebBorderStyle](../../../aspose.cells.gridweb/webborderstyle/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


