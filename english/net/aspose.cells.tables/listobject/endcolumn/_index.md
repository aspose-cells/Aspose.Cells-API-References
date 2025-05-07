---
title: ListObject.EndColumn
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the end column of the range
type: docs
url: /net/aspose.cells.tables/listobject/endcolumn/
---
## ListObject.EndColumn property

Gets the end column of the range.

```csharp
public int EndColumn { get; }
```

### Examples

```csharp
// Called: table.Resize(table.StartRow, table.StartColumn, 6, table.EndColumn, true);
[Test]
        public void Property_EndColumn()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA42093.xlsx");
            Worksheet sheet = workbook.Worksheets["S.02.02.01 Inv"];
            ListObject table = sheet.ListObjects[("Table5")];
            table.Resize(table.StartRow, table.StartColumn, 6, table.EndColumn, true);
            Assert.AreEqual(sheet.Cells["C7"].StringValue,"GBP");
            workbook.Save(Constants.destPath + "CELLSJAVA42093.xlsx");
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


