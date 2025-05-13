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
public void XlsbSaveOptions_Constructor()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells["A1"].PutValue("A1");
    cells["B1"].PutValue("B1");
    cells["C1"].PutValue("C1");
    XlsbSaveOptions saveOptions = new XlsbSaveOptions();
    saveOptions.ExportAllColumnIndexes = true;
    workbook.Save(Constants.destPath + "example.xlsb", saveOptions);
    saveOptions.ExportAllColumnIndexes = false;
    workbook.Save(Constants.destPath + "example.xlsb", saveOptions);
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


