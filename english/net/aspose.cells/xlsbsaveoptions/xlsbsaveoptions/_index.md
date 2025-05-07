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
// Called: wb = Util.ReSave(wb, new XlsbSaveOptions(),
[Test]
        public void XlsbSaveOptions_Constructor()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].SetSharedFormula("=B1", 10, 1);
            wb = Util.ReSave(wb, new XlsbSaveOptions(),
                new LoadOptions() { LightCellsDataHandler = new LightCellsDataHandlerNone() });
            cells = wb.Worksheets[0].Cells;
            for (int i = 0; i < 10; i++)
            {
                Assert.AreEqual("=B" + (i + 1), cells[i, 0].Formula);
            }
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


