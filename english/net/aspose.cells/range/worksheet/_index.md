---
title: Range.Worksheet
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the Worksheetobject which contains this range
type: docs
url: /net/aspose.cells/range/worksheet/
---
## Range.Worksheet property

Gets the `Worksheet`object which contains this range.

```csharp
public Worksheet Worksheet { get; }
```

### Examples

```csharp
// Called: wb.Worksheets.ActiveSheetIndex = rng.Worksheet.Index;
private void Property_Worksheet(string nameText)
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsJava43519.xlsx&quot;);

            Name xlName = wb.Worksheets.Names[nameText];
            Aspose.Cells.Range rng = xlName.GetRange();

            CellArea area = CellArea.CreateCellArea(rng.FirstRow, rng.FirstColumn,
                                                    rng.FirstRow + rng.RowCount - 1,
                                                    rng.FirstColumn + rng.ColumnCount - 1);

            wb.Worksheets.ActiveSheetIndex = rng.Worksheet.Index;

            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);

            options.HtmlCrossStringType = (HtmlCrossType.Cross);
            options.PresentationPreference = (true);
            options.ExportHiddenWorksheet = (false);
            options.ExportActiveWorksheetOnly = (true);
            options.ExportImagesAsBase64 = (true);
            options.CreateDirectory = (false);
            options.ExcludeUnusedStyles = (true);
            options.ExportDocumentProperties = (false);
            options.ExportWorksheetProperties = (false);
            options.ExportBogusRowData = (false);
            options.ExportFrameScriptsAndProperties = (false);
            options.ValidateMergedAreas = (true);

            // NOTE: We are removing hidden ROWS/COLS
            options.HiddenColDisplayType = (HtmlHiddenColDisplayType.Remove);
            options.HiddenRowDisplayType = (HtmlHiddenRowDisplayType.Remove);

            options.ExportArea = (area);
            wb.Save(Constants.destPath + &quot;CellsJava43519-&quot;+nameText+&quot;.html&quot;, options);
        }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


