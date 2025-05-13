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
public void WorkbookDesigner_Method_GetSmartMarkers()
{
    FileStream stream = File.OpenRead(Constants.sourcePath + "example.xls");
    byte[] buffer = new byte[stream.Length];
    stream.Read(buffer, 0, buffer.Length);

    WorkbookDesigner wd = new WorkbookDesigner();
    using (MemoryStream templateStream = new MemoryStream(buffer))
    {
        wd.Workbook = new Workbook(templateStream);        //  Fetch template
        //wd.Workbook.Open(stream);
    }

    string[] smartmarkers = wd.GetSmartMarkers();

    DataTable datasource = new DataTable("COLORS_TIMES");

    datasource.Columns.Add("COLORS", typeof(string));
    datasource.Columns.Add("TIMES", typeof(DateTime));
    DateTime dt = DateTime.Now;
    datasource.Rows.Add(new object[] { "red", dt.AddDays(-1) });
    datasource.Rows.Add(new object[] { "yellow", dt });
    datasource.Rows.Add(new object[] { "green", dt.AddDays(+1) });

    wd.SetDataSource(datasource.DefaultView);

    wd.Process();
    Cells cells = wd.Workbook.Worksheets[0].Cells;
    Assert.AreEqual(cells["A2"].StringValue, "red");
    Assert.AreEqual(cells["A4"].StringValue, "yellow");
    Assert.AreEqual(cells["A6"].StringValue, "green");
    Assert.AreEqual(cells["C1"].DoubleValue,CellsHelper.GetDoubleFromDateTime(dt,false));
    wd.Workbook.Save(Constants.destPath + "example.xls");

}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


