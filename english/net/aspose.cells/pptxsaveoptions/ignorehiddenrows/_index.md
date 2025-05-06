---
title: PptxSaveOptions.IgnoreHiddenRows
second_title: Aspose.Cells for .NET API Reference
description: PptxSaveOptions property. Inidicates whether ignoring hidden rows when converting Excel to PowerPoint
type: docs
url: /net/aspose.cells/pptxsaveoptions/ignorehiddenrows/
---
## PptxSaveOptions.IgnoreHiddenRows property

Inidicates whether ignoring hidden rows when converting Excel to PowerPoint.

```csharp
public bool IgnoreHiddenRows { get; set; }
```

### Examples

```csharp
// Called: saveOptions.IgnoreHiddenRows = true;
[Test]
        public void Property_IgnoreHiddenRows()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET54753.xlsx&quot;);
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;
            wb.Save(Constants.destPath + &quot;CELLSNET54753.pptx&quot;, saveOptions);
            string slide1 = GetEntryText(Constants.destPath + &quot;CELLSNET54753.pptx&quot;, @&quot;ppt\slides\slide1.xml&quot;);
            Assert.IsTrue(slide1.IndexOf(&quot;Qtr1&quot;) == -1);
        }
```

### See Also

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


