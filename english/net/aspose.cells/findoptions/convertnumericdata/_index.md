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
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet40139.xls&quot;);
            Worksheet ws = wb.Worksheets[0];
            FindOptions options = new FindOptions();
            options.ConvertNumericData = true;
            Cells cells = ws.Cells;
            Cell cell = cells.Find(&quot;01/28/2010&quot;, null, options);
            Assert.AreEqual(cell.Name, &quot;AE2&quot;);
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


