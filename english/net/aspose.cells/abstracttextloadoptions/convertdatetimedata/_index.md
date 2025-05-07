---
title: AbstractTextLoadOptions.ConvertDateTimeData
second_title: Aspose.Cells for .NET API Reference
description: AbstractTextLoadOptions property. Gets or sets a value that indicates whether the string in text file is converted to date data
type: docs
url: /net/aspose.cells/abstracttextloadoptions/convertdatetimedata/
---
## AbstractTextLoadOptions.ConvertDateTimeData property

Gets or sets a value that indicates whether the string in text file is converted to date data.

```csharp
public bool ConvertDateTimeData { get; set; }
```

### Examples

```csharp
// Called: opts.ConvertDateTimeData = false;
[Test]
        public void Property_ConvertDateTimeData()
        {
            TxtLoadOptions opts = new TxtLoadOptions();
            opts.Separator = ';';
            opts.ConvertDateTimeData = false;
            opts.LightCellsDataHandler = new CsvParser();
            Workbook wb = CSVTest.LoadAsCsv("NOM;DATE;VALUE\nXavier;18/06/2023;test\nEric;25/07/2023;test2", opts);
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[1, 1];
            Assert.AreEqual(CellValueType.IsDateTime, cell.Type, "B2.Type");
            Assert.AreEqual("18/06/2023", cell.StringValue, "B2.StringValue");
            cell = cells[2, 1];
            Assert.AreEqual(CellValueType.IsDateTime, cell.Type, "B3.Type");
            Assert.AreEqual("25/07/2023", cell.StringValue, "B3.StringValue");
        }
```

### See Also

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


