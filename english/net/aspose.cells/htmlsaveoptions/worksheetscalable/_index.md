---
title: HtmlSaveOptions.WorksheetScalable
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if zooming in or out the html via worksheet zoom level when saving file to html the default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/worksheetscalable/
---
## HtmlSaveOptions.WorksheetScalable property

Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.

```csharp
public bool WorksheetScalable { get; set; }
```

### Examples

```csharp
// Called: saveOptions.WorksheetScalable = true;
[Test]
        public void  Property_WorksheetScalable()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSJAVA-46068.xlsx&quot;);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.ExportActiveWorksheetOnly = false;
            saveOptions.ExportHiddenWorksheet = false;
            saveOptions.ExcludeUnusedStyles = false;
            saveOptions.ExportWorksheetCSSSeparately = true;
            saveOptions.SaveAsSingleFile = true;
            saveOptions.ExportSingleTab = true;
            saveOptions.ExportPrintAreaOnly = true;
            saveOptions.ExportCellCoordinate = true;
            saveOptions.HtmlCrossStringType = HtmlCrossType.Cross;
            saveOptions.WorksheetScalable = true;
            saveOptions.ExportSimilarBorderStyle = true;

            wb.Save(_destFilesPath + &quot;CELLSJAVA-46068.html&quot;, saveOptions);
            wb = new Workbook(_destFilesPath + &quot;CELLSJAVA-46068.html&quot;);
            //wb.Save(_destFilesPath + &quot;CELLSJAVA-46068.xlsx&quot;);
            Cells cells= wb.Worksheets[0].Cells;
            Assert.AreEqual(CellBorderType.Thin,cells[&quot;t2&quot;].GetStyle().Borders[BorderType.RightBorder].LineStyle );
            Assert.AreEqual(CellBorderType.Thin,cells[&quot;u2&quot;].GetStyle().Borders[BorderType.RightBorder].LineStyle );
            Assert.AreEqual(CellBorderType.None,cells[&quot;v2&quot;].GetStyle().Borders[BorderType.RightBorder].LineStyle );
            Assert.AreEqual(CellBorderType.Thin,cells[&quot;t3&quot;].GetStyle().Borders[BorderType.RightBorder].LineStyle);
            Assert.AreEqual(CellBorderType.Thin,cells[&quot;u3&quot;].GetStyle().Borders[BorderType.RightBorder].LineStyle);
            Assert.AreEqual(CellBorderType.None, cells[&quot;v3&quot;].GetStyle().Borders[BorderType.RightBorder].LineStyle);
            Assert.AreEqual(CellBorderType.Thin, cells[&quot;t4&quot;].GetStyle().Borders[BorderType.RightBorder].LineStyle);
            Assert.AreEqual(CellBorderType.Thin, cells[&quot;u4&quot;].GetStyle().Borders[BorderType.RightBorder].LineStyle);
            Assert.AreEqual(CellBorderType.None, cells[&quot;v4&quot;].GetStyle().Borders[BorderType.RightBorder].LineStyle);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


