---
title: PaginatedSaveOptions.IsFontSubstitutionCharGranularity
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Indicates whether to only substitute the font of character when the cell font is not compatibility for it
type: docs
url: /net/aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/
---
## PaginatedSaveOptions.IsFontSubstitutionCharGranularity property

Indicates whether to only substitute the font of character when the cell font is not compatibility for it.

```csharp
public bool IsFontSubstitutionCharGranularity { get; set; }
```

### Remarks

Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

### Examples

```csharp
// Called: IsFontSubstitutionCharGranularity = true,
public static void Property_IsFontSubstitutionCharGranularity()
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

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


