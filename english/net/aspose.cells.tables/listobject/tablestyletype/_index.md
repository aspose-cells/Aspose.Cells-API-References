---
title: TableStyleType
second_title: Aspose.Cells for .NET API Reference
description: Gets and the built-in table style.
type: docs
weight: 210
url: /net/aspose.cells.tables/listobject/tablestyletype/
---
## ListObject.TableStyleType property

Gets and the built-in table style.

```csharp
public TableStyleType TableStyleType { get; set; }
```

### Examples

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

### See Also

* enum [TableStyleType](../../tablestyletype)
* class [ListObject](../../listobject)
* namespace [Aspose.Cells.Tables](../../listobject)
* assembly [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
