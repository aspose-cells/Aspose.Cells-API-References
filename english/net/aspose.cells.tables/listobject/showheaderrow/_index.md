---
title: ListObject.ShowHeaderRow
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets whether this ListObject show header row
type: docs
url: /net/aspose.cells.tables/listobject/showheaderrow/
---
## ListObject.ShowHeaderRow property

Gets and sets whether this ListObject show header row.

```csharp
public bool ShowHeaderRow { get; set; }
```

### Examples

```csharp
// Called: if (table.ShowHeaderRow)
[Test]
        public void Property_ShowHeaderRow()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsJava41707.xlsx&quot;);
            String worksheetName = &quot;Sheet1&quot;;
            String tableName = &quot;Table1&quot;;
            Worksheet worksheet = workbook.Worksheets[worksheetName];
            Aspose.Cells.Font f = worksheet.Cells[&quot;B3&quot;].GetStyle().Font;
            //workbook.Save(path + &quot;dest.pdf&quot;);
            //workbook.Save(path + &quot;dest.xlsx&quot;);
            //return;
            //workbook.calculateFormula(); 
            ListObject table = worksheet.ListObjects[tableName];

            Worksheet newWorksheet = table.DataRange.Worksheet;
            Aspose.Cells.Range sourceRange = table.DataRange;
            if (table.ShowHeaderRow)
            {
                //Include table&apos;s header row 
                int fcol = sourceRange.FirstColumn;
                int frow = sourceRange.FirstRow - 1;
                // including the first header row. 
                int rowCount = sourceRange.RowCount + 1;
                // including the first header row. 
                int colCount = sourceRange.ColumnCount;
                sourceRange = newWorksheet.Cells.CreateRange(frow, fcol, rowCount, colCount);
            }

            Workbook newWorkbook = new Workbook(FileFormatType.Xlsx);
            WorksheetCollection targetWsc = newWorkbook.Worksheets;
            Worksheet targetWs = (Worksheet)targetWsc[0];

            Aspose.Cells.Range targetRange = targetWs.Cells.CreateRange(0, 0, sourceRange.RowCount, sourceRange.ColumnCount);

            PasteOptions options = new PasteOptions();
            //Copy everything else 
            options.PasteType = (PasteType.All);

            targetRange.Copy(sourceRange, options);
            f = newWorkbook.Worksheets[0].Cells[&quot;A1&quot;].GetStyle().Font;
            AssertHelper.AreEqual(f.Color,System.Drawing.Color.Black);
            Util.ReSave(newWorkbook, SaveFormat.Xlsx);
            Util.SaveAsBuffer(newWorkbook, SaveFormat.Pdf);
            //newWorkbook.Save(Constants.destPath + &quot;CellsJava41707_41706_41705.xlsx&quot;);
            //newWorkbook.Save(Constants.destPath + &quot;CellsJava41707_41706_41705.pdf&quot;);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


