---
title: HtmlLoadOptions.HtmlLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions constructor. Creates an options of loading the file
type: docs
url: /net/aspose.cells/htmlloadoptions/htmlloadoptions/
---
## HtmlLoadOptions() {#constructor}

Creates an options of loading the file.

```csharp
public HtmlLoadOptions()
```

### Examples

```csharp
// Called: HtmlLoadOptions loadOptions = new HtmlLoadOptions();
public void HtmlLoadOptions_Constructor()
        {
          //  Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSNET-55291.xlsx&quot;);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.XHtml);
          //  wb.Save(_destFilesPath + &quot;CELLSNET-55291.xhtml&quot;, saveOptions);
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
         //    Workbook wb2 = new Workbook(_destFilesPath + &quot;CELLSNET-55291.xhtml&quot;);
          // wb2.Save(_destFilesPath + &quot;CELLSNET-55291_output.xlsx&quot;);
            CompareOption compareOption = new CompareOption();
            compareOption.CellProperty = false;
            compareOption.CustomProperty = true;
            compareOption.WorkbookProperty = true;
            compareOption.HyperlinkProperty = true;
            compareOption.CellValue = true;
          //  CompareAction.Compare(wb, wb2, compareOption);
          var  wb = new Workbook(Constants.HtmlPath + &quot;CELLSNET-55291-2.xlsx&quot;);
         //   wb.Save(_destFilesPath + &quot;CELLSNET-55291-2.html&quot;, saveOptions);
           var wb2 = new Workbook(_destFilesPath + &quot;CELLSNET-55291-2.xhtml&quot;);
            wb2.Save(_destFilesPath + &quot;CELLSNET-55291-2_output.xlsx&quot;);
            CompareAction.Compare(wb, wb2, compareOption);
        }
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlLoadOptions(LoadFormat) {#constructor_1}

Creates an options of loading the file.

```csharp
public HtmlLoadOptions(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format. |

### See Also

* enum [LoadFormat](../../loadformat/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


