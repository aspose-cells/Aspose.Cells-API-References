---
title: "PivotCache.SourceCellArea"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotCache 属性。返回使用 SourceSheet 的数据源范围"
type: docs
url: /zh/net/aspose.cells.gridweb.data/pivotcache/sourcecellarea/
---
## PivotCache.SourceCellArea property

返回使用 SourceSheet 的数据源范围。

```csharp
public WebCellArea SourceCellArea { get; }
```

### 示例

```csharp

 [C#]

 //更改数据源范围
 //原始值：StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 PivotTable table = GridWeb1.WebWorksheets.PivotTables["myPivotTable"];
 //添加 2 行数据
 table.PivotCache.SourceCellArea.EndRow = 12;

 [VB]

 'Changes data source range
 'Original value: StartRow=0;StartColumn=0;EndRow=10;EndColumn=4;
 Dim table As PivotTable =  GridWeb1.WebWorksheets.PivotTables("myPivotTable")
  'Adds 2 row data
 table.PivotCache.SourceCellArea.EndRow = 12
```

### 另请参见

* class [WebCellArea](../../webcellarea/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


