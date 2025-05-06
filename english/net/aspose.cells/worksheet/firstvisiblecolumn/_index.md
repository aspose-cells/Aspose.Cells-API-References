---
title: Worksheet.FirstVisibleColumn
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents first visible column index
type: docs
url: /net/aspose.cells/worksheet/firstvisiblecolumn/
---
## Worksheet.FirstVisibleColumn property

Represents first visible column index.

```csharp
public int FirstVisibleColumn { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(wb.Worksheets[2].FirstVisibleColumn);
[Test]
        public void Property_FirstVisibleColumn()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET47593/&quot;;
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(filePath + &quot;AS-ISK_v2_1.xlsm&quot;);
            Console.WriteLine(wb.Worksheets[2].FirstVisibleColumn);
            Console.WriteLine(wb.Worksheets[2].FirstVisibleRow);

            //wb.Save(filePath + &quot;out.xlsx&quot;);
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExcludeUnusedStyles = true;
            options.ExportActiveWorksheetOnly = true;
            //options.ExportWorkbookProperties = false;
            //options.ExportWorksheetProperties = false;
            wb.Worksheets.ActiveSheetIndex = 2;

            wb.Save(savePath + &quot;out.html&quot;, options);

            Workbook workbook = new Workbook(filePath + &quot;sample.htm&quot;, new Aspose.Cells.HtmlLoadOptions());
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


