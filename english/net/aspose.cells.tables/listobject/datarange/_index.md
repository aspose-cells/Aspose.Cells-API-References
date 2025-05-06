---
title: ListObject.DataRange
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the data range of the ListObject
type: docs
url: /net/aspose.cells.tables/listobject/datarange/
---
## ListObject.DataRange property

Gets the data range of the ListObject.

```csharp
public Range DataRange { get; }
```

### Examples

```csharp
// Called: Worksheet newWorksheet = table.DataRange.Worksheet;
[Test]
	    public void Property_DataRange()
	    {
            String worksheetName = &quot;Sheet1&quot;;
            String tableName = &quot;Table1&quot;;
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42278.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[worksheetName];
            ListObject table = worksheet.ListObjects[tableName];
            Worksheet newWorksheet = table.DataRange.Worksheet;
            int rowCount = 0;
            Aspose.Cells.Range sourceRange = table.DataRange;
            if (table.ShowHeaderRow)
            {
                //Include table&apos;s header row 
                int fcol = sourceRange.FirstColumn;
                int frow = sourceRange.FirstRow - 1;
                // including the first header row. 
                rowCount = sourceRange.RowCount + 1;
                // including the first header row. 
                int colCount = sourceRange.ColumnCount;
                sourceRange = newWorksheet.Cells.CreateRange(frow, fcol, rowCount, colCount);
            }

            Workbook newWorkbook = new Workbook(FileFormatType.Xlsx);
            newWorkbook.DefaultStyle = (workbook.DefaultStyle);
            WorksheetCollection targetWsc = newWorkbook.Worksheets;
            Worksheet targetWs = (Worksheet)targetWsc[0];
            Aspose.Cells.Range targetRange = targetWs.Cells.CreateRange(0, 0, sourceRange.RowCount,
            sourceRange.ColumnCount);
            PasteOptions options = new PasteOptions();
            //Copy column widths
            options.PasteType = (PasteType.ColumnWidths);
            targetRange.Copy(sourceRange, options);

            // Copy row heights
            rowCount = sourceRange.RowCount;
            int firstRow = sourceRange.FirstRow;
            //for (int i = 0; i &lt; rowCount; i++)
            //{
            //    double rowHeight = sourceRange.Worksheet().getCells().getRowHeight(firstRow++);
            //    targetWs.getCells().setRowHeight(i, rowHeight);
            //}

            //Copy everything else
            options.PasteType = (PasteType.All);
            targetRange.Copy(sourceRange, options);
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            //htmlSaveOptions.HiddenColDisplayType=(1);
            //htmlSaveOptions.HiddenRowDisplayType=(1);
            //htmlSaveOptions.ParseHtmlTagInCell=(true);
            newWorkbook.Save(Constants.destPath + &quot;CELLSJAVA42278.html&quot;, htmlSaveOptions);
	    }
```

### See Also

* class [Range](../../../aspose.cells/range/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


