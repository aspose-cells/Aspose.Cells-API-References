---
title: LoadOptions.LightCellsDataHandler
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. The data handler for processing cells data when reading template file
type: docs
url: /net/aspose.cells/loadoptions/lightcellsdatahandler/
---
## LoadOptions.LightCellsDataHandler property

The data handler for processing cells data when reading template file.

```csharp
public LightCellsDataHandler LightCellsDataHandler { get; set; }
```

### Examples

```csharp
// Called: opts.LightCellsDataHandler = new DataTableExporter(dt);
public void LoadOptions_Property_LightCellsDataHandler()
{
    DataTable dt = new DataTable();
    dt.Columns.Add("Column1", typeof(string));
    dt.Columns.Add("Column2", typeof(DateTime));
    dt.Columns.Add("Column3", typeof(double));
    TxtLoadOptions opts = new TxtLoadOptions();
    opts.ConvertDateTimeData = false;
    opts.ConvertNumericData = false;
    opts.LightCellsDataHandler = new DataTableExporter(dt);
    Workbook wb = CSVTest.LoadAsCsv("row1,06/18/2023,1234.5\nrow2,07/25/2023,5678.9", opts);
    Assert.AreEqual(2, dt.Rows.Count, "Total rows of data");
    Assert.AreEqual("row1", dt.Rows[0][0]);
    Assert.AreEqual("row2", dt.Rows[1][0]);
    Assert.AreEqual("18/06/2023", ((DateTime)dt.Rows[0][1]).ToString("dd/MM/yyyy"));
    Assert.AreEqual("25/07/2023", ((DateTime)dt.Rows[1][1]).ToString("dd/MM/yyyy"));
    Assert.AreEqual(1236.5, dt.Rows[0][2]);
    Assert.AreEqual(5680.9, dt.Rows[1][2]);
}
```

### See Also

* interface [LightCellsDataHandler](../../lightcellsdatahandler/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


