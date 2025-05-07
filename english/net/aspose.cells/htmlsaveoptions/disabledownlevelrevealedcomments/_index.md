---
title: HtmlSaveOptions.DisableDownlevelRevealedComments
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if disable Downlevelrevealed conditional comments when exporting file to html the default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/
---
## HtmlSaveOptions.DisableDownlevelRevealedComments property

Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false.

```csharp
public bool DisableDownlevelRevealedComments { get; set; }
```

### Examples

```csharp
// Called: options.DisableDownlevelRevealedComments = true;
[Test]
        public void Property_DisableDownlevelRevealedComments()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET45357/";
            Workbook wb = new Workbook(filePath + "a.xlsx");
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.DisableDownlevelRevealedComments = true;
            wb.Save(CreateFolder(filePath) + "out.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


