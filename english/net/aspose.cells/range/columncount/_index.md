---
title: Range.ColumnCount
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the count of columns in the range
type: docs
url: /net/aspose.cells/range/columncount/
---
## Range.ColumnCount property

Gets the count of columns in the range.

```csharp
public int ColumnCount { get; }
```

### Examples

```csharp
// Called: Aspose.Cells.Range targetRange = targetWs.Cells.CreateRange(0, 0, sourceRange.RowCount, sourceRange.ColumnCount);
[Test]
        public void Property_ColumnCount()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA42162AndJava42164And42165/&quot;;

            string savePath = CreateFolder(filePath);
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
            htmlSaveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove;

            //CELLSJAVA-42162: Data loss for the range BWY_LandscapeTable2.
            //CELLSJAVA-42164: Data loss for the range TestLandscape.
            //CELLSJAVA-42165: Data loss for the range NewTestForMichele.
            //JAVA-42162 //- BWY_LandscapeTable2 - Data is lost after row 2
            //JAVA-42164 //- TestLandscape - Data is lost from row 36 to row 61
            //JAVA-42165 //- NewTestForMichele - Data is lost after row 65
            string[] ranges = { &quot;BWY_LandscapeTable2&quot;, &quot;TestLandscape&quot;, &quot;NewTestForMichele&quot; };
            foreach (string rangeName in ranges)
            {
                Workbook workbook = new Workbook(filePath + &quot;DataWithHiddenRowsColumns.xlsm&quot;);

                Aspose.Cells.Range sourceRange = workbook.Worksheets.GetRangeByName(rangeName);
                Console.WriteLine(sourceRange.ToString());
                Workbook newWorkbook = new Workbook(FileFormatType.Xlsx);
                newWorkbook.DefaultStyle = sourceRange.Worksheet.Workbook.DefaultStyle;
                WorksheetCollection targetWsc = newWorkbook.Worksheets;
                Worksheet targetWs = targetWsc[0];
                Aspose.Cells.Range targetRange = targetWs.Cells.CreateRange(0, 0, sourceRange.RowCount, sourceRange.ColumnCount);
                PasteOptions options = new PasteOptions();
                options.PasteType = PasteType.ColumnWidths;
                targetRange.Copy(sourceRange, options);
                int rowCount = sourceRange.RowCount;
                int firstRow = sourceRange.FirstRow;

                for (int i = 0; i &lt; rowCount; i++)
                {
                    double rowHeight = sourceRange.Worksheet.Cells.GetRowHeight(firstRow++);
                    targetWs.Cells.SetRowHeight(i, rowHeight);
                }
                options.PasteType = PasteType.All;
                targetRange.Copy(sourceRange, options);

                newWorkbook.Save(savePath + rangeName + &quot;_out.html&quot;, htmlSaveOptions);
            }
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


