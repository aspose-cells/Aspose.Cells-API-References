---
title: XlsbSaveOptions.XlsbSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: XlsbSaveOptions constructor. Creates xlsb file save options
type: docs
url: /net/aspose.cells/xlsbsaveoptions/xlsbsaveoptions/
---
## XlsbSaveOptions() {#constructor}

Creates xlsb file save options.

```csharp
public XlsbSaveOptions()
```

### Examples

```csharp
// Called: XlsbSaveOptions saveOptions = new XlsbSaveOptions();
[Test]
        public void XlsbSaveOptions_Constructor()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;A1&quot;].PutValue(&quot;A1&quot;);
            cells[&quot;B1&quot;].PutValue(&quot;B1&quot;);
            cells[&quot;C1&quot;].PutValue(&quot;C1&quot;);
            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.ExportAllColumnIndexes = true;
            workbook.Save(Constants.destPath + &quot;ExportColumnIndexes001.xlsb&quot;, saveOptions);
            saveOptions.ExportAllColumnIndexes = false;
            workbook.Save(Constants.destPath + &quot;ExportColumnIndexes002.xlsb&quot;, saveOptions);
        }
```

### See Also

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsbSaveOptions(SaveFormat) {#constructor_1}

Creates xlsb file save options.

```csharp
[Obsolete("Use XlsbSaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public XlsbSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The save format . It must be xlsb. |

### Remarks

NOTE: This constructor is now obsolete. Instead, please use XlsbSaveOptions() constructor. This property will be removed 12 months later since January 2021. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* enum [SaveFormat](../../saveformat/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


