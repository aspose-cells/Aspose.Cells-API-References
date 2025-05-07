---
title: Range.Merge
second_title: Aspose.Cells for .NET API Reference
description: Range method. Combines a range of cells into a single cell
type: docs
url: /net/aspose.cells/range/merge/
---
## Range.Merge method

Combines a range of cells into a single cell.

```csharp
public void Merge()
```

### Remarks

Reference the merged cell via the address of the upper-left cell in the range.

### Examples

```csharp
// Called: range2.Merge();
[Test]
        public void Method_Merge()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47308/";

            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            string htmlString1 = "<font style=\"font-weight:normal; text-decoration:underline;color:red;\">Red1</font><font style=\"font-weight:normal;text-decoration:underline;color:green;\">Green1</font>";
            var cell1 = ws.Cells[1, 1];
            cell1.HtmlString = htmlString1;

            //string htmlString2 = "<font style=\"font-weight:normal; text-decoration:underline;color:red;\">Red2</font><font style=\"font-weight:normal;text-decoration:underline;color:green;\">Green2</font>";
            var cell2 = ws.Cells[3, 1];
            cell2.HtmlString = htmlString1;
            var range2 = ws.Cells.CreateRange(3, 1, 5, 5);
            range2.Merge();
            XlsSaveOptions saveOptions = new XlsSaveOptions();

            string savePath = CreateFolder(filePath);
            wb.Save(savePath + @"out.xls", saveOptions);

            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            wb.Save(savePath + @"out.htm", htmlSaveOptions);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


