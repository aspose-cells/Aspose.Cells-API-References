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
// Called: wb = new Workbook(filePath + "LKaw.html", new Aspose.Cells.HtmlLoadOptions());
[Test]
        public void HtmlLoadOptions_Constructor()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47682AndNET47684And47685/";

            Workbook wb = null;
            wb = new Workbook(filePath + "ret_report07.htm", new Aspose.Cells.HtmlLoadOptions());
            //wb = new Workbook(filePath + "R_GC_CC_MATERIAL_BAL_BATCH.htm", new Aspose.Cells.HtmlLoadOptions());
            wb = new Workbook(filePath + "LKaw.html", new Aspose.Cells.HtmlLoadOptions());
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


