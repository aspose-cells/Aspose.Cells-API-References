---
title: Worksheet.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents if the worksheet is visible
type: docs
url: /net/aspose.cells/worksheet/isvisible/
---
## Worksheet.IsVisible property

Represents if the worksheet is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
// Called: book.Worksheets[&amp;quot;工作表2&amp;quot;].IsVisible = false;
[Test]
        public void Property_IsVisible()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA42277/&quot;;

            String fileName = &quot;PusheenVisio-20170427.xlsx&quot;;

            Workbook book = new Workbook(filePath + fileName);

            book.Worksheets[&quot;工作表2&quot;].IsVisible = false;
            book.Worksheets[&quot;工作表3&quot;].IsVisible = false;

            HtmlSaveOptions saveOps = new HtmlSaveOptions();
            saveOps.ClearData = false;
            saveOps.CreateDirectory = false;
            saveOps.ExportActiveWorksheetOnly = false;
            saveOps.ExportHiddenWorksheet = false;
            ; //Comment this line and image will display fine
            saveOps.ParseHtmlTagInCell = true;
            saveOps.Encoding = Encoding.UTF8;
            saveOps.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove;
            saveOps.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
            saveOps.ExportImagesAsBase64 = true;
            book.Save(_destFilesPath + &quot;JAVA42277.html&quot;, saveOps);
            book = new Workbook(_destFilesPath + &quot;JAVA42277.html&quot;);
            Assert.AreEqual(book.Worksheets.Count, 1);
            Assert.AreEqual(book.Worksheets[0].Shapes.Count, 2);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


