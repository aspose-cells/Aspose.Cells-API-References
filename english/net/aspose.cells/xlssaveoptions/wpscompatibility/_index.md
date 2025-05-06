---
title: XlsSaveOptions.WpsCompatibility
second_title: Aspose.Cells for .NET API Reference
description: XlsSaveOptions property. Indicates whether to make the xls more compatible with WPS
type: docs
url: /net/aspose.cells/xlssaveoptions/wpscompatibility/
---
## XlsSaveOptions.WpsCompatibility property

Indicates whether to make the xls more compatible with WPS.

```csharp
public bool WpsCompatibility { get; set; }
```

### Examples

```csharp
// Called: saveOptions.WpsCompatibility = true;
[Test]
        public void Property_WpsCompatibility()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet56669.xls&quot;);
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.WpsCompatibility = true;
            workbook.Save(Constants.destPath + &quot;CellsNet56669.xls&quot;, saveOptions);

        }
```

### See Also

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


