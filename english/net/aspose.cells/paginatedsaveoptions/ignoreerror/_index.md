---
title: PaginatedSaveOptions.IgnoreError
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Indicates if you need to hide the error while rendering. The error can be error in shape image chart rendering etc
type: docs
url: /net/aspose.cells/paginatedsaveoptions/ignoreerror/
---
## PaginatedSaveOptions.IgnoreError property

Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.

```csharp
public bool IgnoreError { get; set; }
```

### Examples

```csharp
// Called: IgnoreError = false,
public static void Property_IgnoreError()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].PutValue(123);

            // Create XpsSaveOptions with specific settings
            XpsSaveOptions saveOptions = new XpsSaveOptions
            {
                DefaultFont = "Arial",
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
            workbook.Save("XpsSaveOptionsExample.xps", saveOptions);
        }
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


