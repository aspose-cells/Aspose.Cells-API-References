---
title: XpsSaveOptions.XpsSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: XpsSaveOptions constructor. Creates options for saving xps file
type: docs
url: /net/aspose.cells/xpssaveoptions/xpssaveoptions/
---
## XpsSaveOptions() {#constructor}

Creates options for saving xps file.

```csharp
public XpsSaveOptions()
```

### Examples

```csharp
// Called: XpsSaveOptions saveOptions = new XpsSaveOptions
public static void XpsSaveOptions_Constructor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello&quot;);
            sheet.Cells[&quot;A2&quot;].PutValue(&quot;World&quot;);
            sheet.Cells[&quot;A3&quot;].PutValue(123);

            // Create XpsSaveOptions with specific settings
            XpsSaveOptions saveOptions = new XpsSaveOptions
            {
                DefaultFont = &quot;Arial&quot;,
                CheckWorkbookDefaultFont = true,
                CheckFontCompatibility = true,
                IsFontSubstitutionCharGranularity = true,
                OnePagePerSheet = true,
                AllColumnsInOnePagePerSheet = true,
                IgnoreError = false,
                OutputBlankPageWhenNothingToPrint = false,
                PageIndex = 0,
                PageCount = 1,
                PrintingPageType = PrintingPageType.Default,
                GridlineType = GridlineType.Dotted,
                TextCrossType = TextCrossType.Default,
                DefaultEditLanguage = DefaultEditLanguage.English,
                SheetSet = SheetSet.All
            };

            // Save the workbook as XPS with the specified options
            workbook.Save(&quot;XpsSaveOptionsExample.xps&quot;, saveOptions);
        }
```

### See Also

* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XpsSaveOptions(SaveFormat) {#constructor_1}

Creates options for saving xps file.

```csharp
[Obsolete("Use XpsSaveOptions() constructor instead.")]
public XpsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The save format, it must be xps format. |

### Remarks

NOTE: This constructor is now obsolete. Instead, please use XpsSaveOptions() constructor. This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* enum [SaveFormat](../../saveformat/)
* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


