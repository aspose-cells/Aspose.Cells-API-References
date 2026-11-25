---
title: "AutoFitterOptions.AutoFitWrappedTextType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFitterOptions. Ottiene e imposta il tipo di adattamento automatico del testo a capo"
type: docs
url: /it/net/aspose.cells/autofitteroptions/autofitwrappedtexttype/
---
## AutoFitterOptions.AutoFitWrappedTextType property

Ottiene e imposta il tipo di adattamento automatico del testo a capo.

```csharp
public AutoFitWrappedTextType AutoFitWrappedTextType { get; set; }
```

### Esempi

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
            
            // Accesso a stile fisso usando il modello GetStyle/SetStyle
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

### Vedi anche

* enum [AutoFitWrappedTextType](../../autofitwrappedtexttype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


