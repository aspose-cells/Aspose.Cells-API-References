---
title: "AutoFitterOptions.AutoFitWrappedTextType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFitterOptions-Eigenschaft. Gibt den Typ des automatisch angepassten umgebrochenen Textes zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells/autofitteroptions/autofitwrappedtexttype/
---
## AutoFitterOptions.AutoFitWrappedTextType property

Liest und setzt den Typ der automatischen Anpassung von umgebrochenem Text.

```csharp
public AutoFitWrappedTextType AutoFitWrappedTextType { get; set; }
```

### Beispiele

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
            
            // Fester Stilzugriff mittels GetStyle/SetStyle-Muster
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

### Siehe auch

* enum [AutoFitWrappedTextType](../../autofitwrappedtexttype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


