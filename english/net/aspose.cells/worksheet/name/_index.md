---
title: Worksheet.Name
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets or sets the name of the worksheet
type: docs
url: /net/aspose.cells/worksheet/name/
---
## Worksheet.Name property

Gets or sets the name of the worksheet.

```csharp
public string Name { get; set; }
```

### Remarks

The max length of sheet name is 31. And you cannot assign same name(case insensitive) to two worksheets. For example, you cannot set "SheetName1" to the first worksheet and set "SHEETNAME1" to the second worksheet.

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Tabelle1&amp;quot;, sheet.Name);
[Test]
        public void Property_Name()
        {
            string file = Constants.sourcePath + &quot;TestWorkbook\\Book1.xlsx&quot;;
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            Workbook workbook = new Workbook(file, loadOptions);

            Assert.AreEqual(3, workbook.Worksheets.Count);
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;
            Assert.AreEqual(&quot;Tabelle1&quot;, sheet.Name);
            Assert.AreEqual(&quot;Tabelle1&quot;, cells[1, 1].StringValue);
            Assert.AreEqual(3, cells[3, 2].IntValue);

            sheet = workbook.Worksheets[1];
            cells = sheet.Cells;
            Assert.AreEqual(&quot;Tabelle2&quot;, sheet.Name);
            Assert.AreEqual(&quot;Tabelle2&quot;, cells[1, 1].StringValue);

            sheet = workbook.Worksheets[2];
            cells = sheet.Cells;
            Assert.AreEqual(&quot;Tabelle3&quot;, sheet.Name);
            Assert.AreEqual(&quot;Tabelle3&quot;, cells[1, 1].StringValue);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


