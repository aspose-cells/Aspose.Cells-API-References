---
title: SaveOptions.CreateDirectory
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. If true and the directory does not exist the directory will be automatically created before saving the file
type: docs
url: /net/aspose.cells/saveoptions/createdirectory/
---
## SaveOptions.CreateDirectory property

If true and the directory does not exist, the directory will be automatically created before saving the file.

```csharp
public bool CreateDirectory { get; set; }
```

### Remarks

The default value is false.

### Examples

```csharp
// Called: options.CreateDirectory = false;
[Test]
        public void Property_CreateDirectory()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA41772/&quot;;
            String wbPath = &quot;ForExport.xlsx&quot;;
            Workbook wb = new Workbook(filePath + wbPath);
            NameCollection names = wb.Worksheets.Names;
            Name name = names[&quot;ExportCells&quot;];

            Aspose.Cells.Range rng = name.GetRange();
            Worksheet sheet = rng.Worksheet;
            Cells cells = sheet.Cells;
            int firstCol = rng.FirstColumn;
            int firstRow = rng.FirstRow;
            int maxCol = cells.MaxDisplayRange.ColumnCount;
            int maxRow = cells.MaxDisplayRange.RowCount;

            // HIDE all the rows and columns that are not part of the range (zero-based)
            if (firstCol &gt; 0)
            {
                cells.HideColumns(0, firstCol);
            }
            if (firstCol + rng.ColumnCount &lt; maxCol)
            {
                cells.HideColumns(firstCol + rng.ColumnCount, maxCol);
            }
            if (firstRow &gt; 0)
            {
                cells.HideRows(0, firstRow);
            }
            if (firstRow + rng.RowCount &lt; maxRow)
            {
                cells.HideRows(firstRow + rng.RowCount, maxRow);
            }

            wb.Worksheets.ActiveSheetIndex = sheet.Index;

            // export the worksheet
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            options.Encoding = Encoding.UTF8;

            options.HtmlCrossStringType = HtmlCrossType.Cross;
            options.PresentationPreference = true;
            options.ExportActiveWorksheetOnly = true;
            options.ExportImagesAsBase64 = true;
            options.CreateDirectory = false;
            options.IsExpImageToTempDir = false;
            // Note, HtmlHiddenColDisplayType.REMOVE is used for columns only. 
            // We found a different bug where the hidden columns were showing up
            // in the transformed HTML - even though they are hidden.
            options.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
            wb.Save(CreateFolder(filePath) + &quot;ForExport_out.html&quot;, options);


            wbPath = &quot;HiddenCols.xlsx&quot;; // assumes file is in path            
            wb = new Workbook(filePath + wbPath);
            names = wb.Worksheets.Names;
            name = names[&quot;PartialHidden&quot;];

            rng = name.GetRange();
            sheet = rng.Worksheet;
            cells = sheet.Cells;
            firstCol = rng.FirstColumn;
            firstRow = rng.FirstRow;
            maxCol = cells.MaxDisplayRange.ColumnCount;
            maxRow = cells.MaxDisplayRange.RowCount;

            // HIDE all the rows and columns that are not part of the range (zero-based)
            if (firstCol &gt; 0)
            {
                cells.HideColumns(0, firstCol);
            }
            if (firstCol + rng.ColumnCount &lt; maxCol)
            {
                cells.HideColumns(firstCol + rng.ColumnCount, maxCol);
            }
            if (firstRow &gt; 0)
            {
                cells.HideRows(0, firstRow);
            }
            if (firstRow + rng.RowCount &lt; maxRow)
            {
                cells.HideRows(firstRow + rng.RowCount, maxRow);
            }

            wb.Worksheets.ActiveSheetIndex = sheet.Index;

            // export the worksheet
            options = new HtmlSaveOptions(SaveFormat.Html);
            options.Encoding = Encoding.UTF8;

            options.HtmlCrossStringType = HtmlCrossType.Cross;
            options.PresentationPreference = true;
            options.ExportActiveWorksheetOnly = true;
            options.ExportImagesAsBase64 = true;
            options.CreateDirectory = false;
            options.IsExpImageToTempDir = false;
            // Note, HtmlHiddenColDisplayType.REMOVE is used for columns only. 
            // We found a different bug where the hidden columns were showing up
            // in the transformed HTML - even though they are hidden.
            options.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
            wb.Save(CreateFolder(filePath) + &quot;HiddenCols_out.html&quot;, options);
        }
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


