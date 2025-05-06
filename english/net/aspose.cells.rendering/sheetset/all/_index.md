---
title: SheetSet.All
second_title: Aspose.Cells for .NET API Reference
description: SheetSet property. Gets a set with all sheets of the workbook in their original order
type: docs
url: /net/aspose.cells.rendering/sheetset/all/
---
## SheetSet.All property

Gets a set with all sheets of the workbook in their original order.

```csharp
public static SheetSet All { get; }
```

### Examples

```csharp
// Called: SheetSet = SheetSet.All
public static void Property_All()
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

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


