---
title: ListColumn.Name
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Gets and sets the name of the column
type: docs
url: /net/aspose.cells.tables/listcolumn/name/
---
## ListColumn.Name property

Gets and sets the name of the column.

```csharp
public string Name { get; set; }
```

### Remarks

If sets the name of the column, the according cell' value will be changed too.

### Examples

```csharp
// Called: Assert.AreEqual("T1",ListObject.ListColumns[0].Name);
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet44076.xls");
            Worksheet worksheet = workbook.Worksheets[0];

            ListObject ListObject = worksheet.ListObjects[0];
            Assert.AreEqual("T1",ListObject.ListColumns[0].Name);
            workbook.Save(Constants.destPath + "CellsNet44076.xls");
            workbook = new Workbook(Constants.destPath + "CellsNet44076.xls");
             worksheet = workbook.Worksheets[0];

            ListObject = worksheet.ListObjects[0];
            Assert.AreEqual("T1", ListObject.ListColumns[0].Name);
        }
```

### See Also

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


