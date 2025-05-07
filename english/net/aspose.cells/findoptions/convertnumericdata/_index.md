---
title: FindOptions.ConvertNumericData
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. Gets or sets a value that indicates whether converting the searched string value to numeric data
type: docs
url: /net/aspose.cells/findoptions/convertnumericdata/
---
## FindOptions.ConvertNumericData property

Gets or sets a value that indicates whether converting the searched string value to numeric data.

```csharp
public bool ConvertNumericData { get; set; }
```

### Examples

```csharp
// Called: options.ConvertNumericData = true;
[Test]
        public void Property_ConvertNumericData()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet40139.xls");
            Worksheet ws = wb.Worksheets[0];
            FindOptions options = new FindOptions();
            options.ConvertNumericData = true;
            Cells cells = ws.Cells;
            Cell cell = cells.Find("01/28/2010", null, options);
            Assert.AreEqual(cell.Name, "AE2");
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


