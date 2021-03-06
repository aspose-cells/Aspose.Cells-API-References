---
title: TableStyleType
second_title: Aspose.Cells for .NET API 参考
description: 获取和内置表格样式
type: docs
weight: 210
url: /zh/net/aspose.cells.tables/listobject/tablestyletype/
---
## ListObject.TableStyleType property

获取和内置表格样式。

```csharp
public TableStyleType TableStyleType { get; set; }
```

### 例子

```csharp

[C#]


Workbook workbook = new Workbook("Book1.xlsx");
ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[0];
table.TableStyleType = TableStyleType.TableStyleDark2;
 workbook.Save("TableStyle.xlsx");
 
[Visual Basic]

Dim workbook As Workbook = New Workbook("Book1.xlsx")
Dim tables As ListObjectCollection = workbook.Worksheets(0).ListObjects
Dim index As Int32 = tables.Add(0, 0, 9, 4, True)
Dim table As ListObject = tables(0)
table.TableStyleType = TableStyleType.TableStyleDark2;
workbook.Save("Book1.xlsx")
```

### 也可以看看

* enum [TableStyleType](../../tablestyletype)
* class [ListObject](../../listobject)
* 命名空间 [Aspose.Cells.Tables](../../listobject)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
