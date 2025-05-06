---
title: HtmlSaveOptions.ShowAllSheets
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether showing all sheets when saving as a single html file
type: docs
url: /net/aspose.cells/htmlsaveoptions/showallsheets/
---
## HtmlSaveOptions.ShowAllSheets property

Indicates whether showing all sheets when saving as a single html file.

```csharp
public bool ShowAllSheets { get; set; }
```

### Remarks

Only works when [`SaveAsSingleFile`](../saveassinglefile/) is True.

### Examples

```csharp
// Called: saveOptions.ShowAllSheets = true;
[Test]
        public void Property_ShowAllSheets()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET51367.xlsx&quot;);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.SaveAsSingleFile = true;
            saveOptions.ShowAllSheets = true;

            saveOptions.ExportPageHeaders = true;
         
            workbook.Save(Constants.destPath + &quot;CellsNet51367.html&quot;, saveOptions);
            string text = File.ReadAllText(Constants.destPath + &quot;CellsNet51367.html&quot;);
            Assert.IsTrue(text.IndexOf(&quot;Sheet 1 - Summary&quot;) != -1);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


