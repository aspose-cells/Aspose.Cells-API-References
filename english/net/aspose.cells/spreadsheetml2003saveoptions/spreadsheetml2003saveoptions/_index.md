---
title: SpreadsheetML2003SaveOptions.SpreadsheetML2003SaveOptions
second_title: Aspose.Cells for .NET API Reference
description: SpreadsheetML2003SaveOptions constructor. Creates the options for saving Excel 2003 spreadml file
type: docs
url: /net/aspose.cells/spreadsheetml2003saveoptions/spreadsheetml2003saveoptions/
---
## SpreadsheetML2003SaveOptions() {#constructor}

Creates the options for saving Excel 2003 spreadml file.

```csharp
public SpreadsheetML2003SaveOptions()
```

### Examples

```csharp
// Called: SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
[Test]
        public void SpreadsheetML2003SaveOptions_Constructor()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells[&quot;AAA1&quot;].PutValue(&quot;dfdf&quot;);
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.LimitAsXls = false;
            workbook.Save(Constants.destPath + &quot;CellsNet25224.xml&quot;,saveOptions);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet25224.xml&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;AAA1&quot;].StringValue, &quot;dfdf&quot;);
        }
```

### See Also

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SpreadsheetML2003SaveOptions(SaveFormat) {#constructor_1}

Creates the options for saving Excel 2003 spreadml file.

```csharp
[Obsolete("Use SpreadsheetML2003SaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SpreadsheetML2003SaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The save format. |

### Remarks

NOTE: This constructor is now obsolete. Instead, please use SpreadsheetML2003SaveOptions() constructor. This property will be removed 12 months later since January 2021. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* enum [SaveFormat](../../saveformat/)
* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


