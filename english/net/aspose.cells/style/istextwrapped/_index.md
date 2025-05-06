---
title: Style.IsTextWrapped
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets a value indicating whether the text within a cell is wrapped
type: docs
url: /net/aspose.cells/style/istextwrapped/
---
## Style.IsTextWrapped property

Gets or sets a value indicating whether the text within a cell is wrapped.

```csharp
public bool IsTextWrapped { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(style.IsTextWrapped);
[Test]
        public void Property_IsTextWrapped()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA42495/&quot;;

            Workbook workbook = new Workbook(filePath + &quot;input.xlsx&quot;);
            HtmlSaveOptions options = new HtmlSaveOptions();
            Worksheet sheet = workbook.Worksheets[&quot;Entry points&quot;];
            workbook.Worksheets.ActiveSheetIndex = sheet.Index;
            options.ExportActiveWorksheetOnly = true;
            options.ExportDocumentProperties = false;
            options.ExportWorkbookProperties = false;
            options.ExportWorksheetProperties = false;
            workbook.Save(Constants.destPath + &quot;JAVA42495.html&quot;, options);

            //simon
            workbook = new Workbook(Constants.destPath + &quot;JAVA42495.html&quot;);
            Style style = workbook.Worksheets[0].Cells[&quot;C3&quot;].GetStyle();
            Assert.IsTrue(style.IsTextWrapped);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


