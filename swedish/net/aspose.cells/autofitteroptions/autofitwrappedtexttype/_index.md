---
title: "AutoFitterOptions.AutoFitWrappedTextType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFitterOptions-egenskap. Hämtar och anger typen av automatisk anpassning av radbruten text"
type: docs
url: /sv/net/aspose.cells/autofitteroptions/autofitwrappedtexttype/
---
## AutoFitterOptions.AutoFitWrappedTextType property

Hämtar och anger typen av automatisk anpassning av radbruten text.

```csharp
public AutoFitWrappedTextType AutoFitWrappedTextType { get; set; }
```

### Exempel

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitWrappedTextTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Cell cell = worksheet.Cells["A1"];
            cell.Value = "This is a sample text string that demonstrates auto-fitting wrapped text using Paragraph mode";
            
            // Fast stilåtkomst med GetStyle/SetStyle-mönster
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            cell.SetStyle(style);
            
            AutoFitterOptions options = new AutoFitterOptions
            {
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            };

            worksheet.AutoFitColumns(options);
            workbook.Save("output.html", SaveFormat.Html);
        }
    }
}
```

### Se även

* enum [AutoFitWrappedTextType](../../autofitwrappedtexttype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


