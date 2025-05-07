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
// Called: pdfSaveOptions.RefreshChartCache = (true);
[Test]
        public void Property_RefreshChartCache()
        {
            Workbook asposeWorkbook = new Workbook(Constants.PivotTableSourcePath + "CELLSJAVA-45879.xlsx");
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.RefreshChartCache = (true);
            //asposeWorkbook.Worksheets.RefreshAll();
            //asposeWorkbook.CalculateFormula();
            //asposeWorkbook.Worksheets[1].Charts[0].RefreshPivotData();


            asposeWorkbook.Save(Constants.PivotTableDestPath + "CELLSJAVA45879.pdf", pdfSaveOptions);
            asposeWorkbook.Save(Constants.PivotTableDestPath + "CELLSJAVA45879.xlsx");
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.PivotTableDestPath + "CELLSJAVA45879.xlsx", "xl/pivotCache/pivotCacheRecords1.xml", new string[] { "v=\"43000000000\"" }, true));
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.PivotTableDestPath + "CELLSJAVA45879.xlsx", "xl/charts/chart1.xml", new string[] { "43000000000" }, true));

        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


