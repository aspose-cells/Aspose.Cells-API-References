---
title: WorkbookDesigner.GetSmartMarkers
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner method. Returns a collection of smart markers in a spreadsheet
type: docs
url: /net/aspose.cells/workbookdesigner/getsmartmarkers/
---
## WorkbookDesigner.GetSmartMarkers method

Returns a collection of smart markers in a spreadsheet.

```csharp
public string[] GetSmartMarkers()
```

### Return Value

A collection of smart markers

### Remarks

A string array is created on every call. The array is sorted and duplicated values are removed.

### Examples

```csharp
// Called: string[] smartmarkers = wd.GetSmartMarkers();
[Test]
        public void Method_GetSmartMarkers()
        {
            FileStream stream = File.OpenRead(Constants.sourcePath + &quot;SmartMarker/CellsNet40073.xls&quot;);
            byte[] buffer = new byte[stream.Length];
            stream.Read(buffer, 0, buffer.Length);

            WorkbookDesigner wd = new WorkbookDesigner();
            using (MemoryStream templateStream = new MemoryStream(buffer))
            {
                wd.Workbook = new Workbook(templateStream);        //  Fetch template
                //wd.Workbook.Open(stream);
            }

            string[] smartmarkers = wd.GetSmartMarkers();

            DataTable datasource = new DataTable(&quot;COLORS_TIMES&quot;);

            datasource.Columns.Add(&quot;COLORS&quot;, typeof(string));
            datasource.Columns.Add(&quot;TIMES&quot;, typeof(DateTime));
            DateTime dt = DateTime.Now;
            datasource.Rows.Add(new object[] { &quot;red&quot;, dt.AddDays(-1) });
            datasource.Rows.Add(new object[] { &quot;yellow&quot;, dt });
            datasource.Rows.Add(new object[] { &quot;green&quot;, dt.AddDays(+1) });

            wd.SetDataSource(datasource.DefaultView);

            wd.Process();
            Cells cells = wd.Workbook.Worksheets[0].Cells;
            Assert.AreEqual(cells[&quot;A2&quot;].StringValue, &quot;red&quot;);
            Assert.AreEqual(cells[&quot;A4&quot;].StringValue, &quot;yellow&quot;);
            Assert.AreEqual(cells[&quot;A6&quot;].StringValue, &quot;green&quot;);
            Assert.AreEqual(cells[&quot;C1&quot;].DoubleValue,CellsHelper.GetDoubleFromDateTime(dt,false));
            wd.Workbook.Save(Constants.destPath + &quot;CellsNet40073.xls&quot;);

        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


