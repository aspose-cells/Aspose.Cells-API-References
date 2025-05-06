---
title: Range.ToString
second_title: Aspose.Cells for .NET API Reference
description: Range method. Returns a string represents the current Range object
type: docs
url: /net/aspose.cells/range/tostring/
---
## Range.ToString method

Returns a string represents the current Range object.

```csharp
public override string ToString()
```

### Examples

```csharp
// Called: Console.WriteLine(rng.ToString());
[Test]
        public void Method_ToString()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA42990/&quot;;

            String file = &quot;AutoFilter.xlsx&quot;;
            Workbook wb = new Workbook(filePath + file);

            Name name = wb.Worksheets.Names[&quot;Range2&quot;];
            Aspose.Cells.Range rng = name.GetRange();
            Console.WriteLine(rng.ToString());
            Cells cells = rng.Worksheet.Cells;

            int firstCol = rng.FirstColumn;
            int firstRow = rng.FirstRow;
            int lastCol = firstCol + rng.ColumnCount;
            int lastRow = firstRow + rng.RowCount;
            int maxCol = cells.MaxDisplayRange.ColumnCount;
            int maxRow = cells.MaxDisplayRange.RowCount;

            // Hide all the rows and columns that are not part of the range
            if (firstCol &gt; 0)
            {
                cells.HideColumns(0, firstCol);
            }
            if (lastCol &lt; maxCol)
            {
                cells.HideColumns(lastCol, maxCol + 1 - lastCol);
            }
            if (firstRow &gt; 0)
            {
                cells.HideRows(0, firstRow);
            }
            if (lastRow &lt; maxRow)
            {
                cells.HideRows(lastRow, maxRow - lastRow);
            }

            // export the worksheet
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            // IMPORTANT: We *must* use REMOVE instead of HIDDEN
            options.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
            options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove;

            wb.Save(CreateFolder(filePath) + &quot;out.html&quot;, options);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


