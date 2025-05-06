---
title: ListObject.ListColumns
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets ListColumns of the ListObject
type: docs
url: /net/aspose.cells.tables/listobject/listcolumns/
---
## ListObject.ListColumns property

Gets ListColumns of the ListObject.

```csharp
public ListColumnCollection ListColumns { get; }
```

### Examples

```csharp
// Called: formula1 = ws.ListObjects[0].ListColumns[2].Formula;
[Test]
        public void Property_ListColumns()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET47219_&quot;;

            Workbook wb = new Workbook(filePath + &quot;a.xlsx&quot;);
            Worksheet ws = wb.Worksheets[0];

            string formula1 = ws.ListObjects[0].ListColumns[2].Formula;
            string formula2 = ws.Cells[2, 3].Formula;
            Assert.AreEqual(formula1, formula2);

            ws.Cells.InsertRows(0, 1, true);
            formula1 = ws.ListObjects[0].ListColumns[2].Formula;
            formula2 = ws.Cells[3, 3].Formula;
            Assert.AreEqual(formula1, formula2);
        }
```

### See Also

* class [ListColumnCollection](../../listcolumncollection/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


