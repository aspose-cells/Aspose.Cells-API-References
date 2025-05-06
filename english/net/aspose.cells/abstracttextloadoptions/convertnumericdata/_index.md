---
title: AbstractTextLoadOptions.ConvertNumericData
second_title: Aspose.Cells for .NET API Reference
description: AbstractTextLoadOptions property. Gets or sets a value that indicates whether the string in text file is converted to numeric data
type: docs
url: /net/aspose.cells/abstracttextloadoptions/convertnumericdata/
---
## AbstractTextLoadOptions.ConvertNumericData property

Gets or sets a value that indicates whether the string in text file is converted to numeric data.

```csharp
public bool ConvertNumericData { get; set; }
```

### Examples

```csharp
// Called: opts.ConvertNumericData = false;
[Test]
        public void Property_ConvertNumericData()
        {
            DataTable dt = new DataTable();
            dt.Columns.Add(&quot;Column1&quot;, typeof(string));
            dt.Columns.Add(&quot;Column2&quot;, typeof(DateTime));
            dt.Columns.Add(&quot;Column3&quot;, typeof(double));
            TxtLoadOptions opts = new TxtLoadOptions();
            opts.ConvertDateTimeData = false;
            opts.ConvertNumericData = false;
            opts.LightCellsDataHandler = new DataTableExporter(dt);
            Workbook wb = CSVTest.LoadAsCsv(&quot;row1,06/18/2023,1234.5\nrow2,07/25/2023,5678.9&quot;, opts);
            Assert.AreEqual(2, dt.Rows.Count, &quot;Total rows of data&quot;);
            Assert.AreEqual(&quot;row1&quot;, dt.Rows[0][0]);
            Assert.AreEqual(&quot;row2&quot;, dt.Rows[1][0]);
            Assert.AreEqual(&quot;18/06/2023&quot;, ((DateTime)dt.Rows[0][1]).ToString(&quot;dd/MM/yyyy&quot;));
            Assert.AreEqual(&quot;25/07/2023&quot;, ((DateTime)dt.Rows[1][1]).ToString(&quot;dd/MM/yyyy&quot;));
            Assert.AreEqual(1236.5, dt.Rows[0][2]);
            Assert.AreEqual(5680.9, dt.Rows[1][2]);
        }
```

### See Also

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


