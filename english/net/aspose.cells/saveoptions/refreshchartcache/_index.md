---
title: SaveOptions.RefreshChartCache
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Indicates whether refreshing chart cache data
type: docs
url: /net/aspose.cells/saveoptions/refreshchartcache/
---
## SaveOptions.RefreshChartCache property

Indicates whether refreshing chart cache data

```csharp
public bool RefreshChartCache { get; set; }
```

### Examples

```csharp
// Called: pdfSaveOptions.RefreshChartCache = true;
public void SaveOptions_Property_RefreshChartCache()
{
    string filePath = Constants.PivotTableSourcePath + @"JAVA43033_";


    LoadOptions loadOptions = new LoadOptions();
    loadOptions.MemorySetting = MemorySetting.MemoryPreference;
    DateTime start = DateTime.Now;
    Workbook workbook = new Workbook(filePath + "Database build_Macro_Locked for sending.xlsm", loadOptions);
    Console.WriteLine(DateTime.Now.Subtract(start).ToString());

    PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
    pdfSaveOptions.OnePagePerSheet = false;
    pdfSaveOptions.RefreshChartCache = true;

    workbook.Save(CreateFolder(filePath) + "out.pdf", pdfSaveOptions);

    Console.WriteLine(DateTime.Now.Subtract(start).ToString());
}
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


