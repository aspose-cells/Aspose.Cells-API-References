---
title: "Enum AutoFitWrappedTextType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.AutoFitWrappedTextType enum. Rappresenta il tipo di testo a capo adattato automaticamente"
type: docs
url: /it/net/aspose.cells/autofitwrappedtexttype/
---
## AutoFitWrappedTextType enumeration

Rappresenta il tipo di adattamento automatico del testo a capo.

```csharp
public enum AutoFitWrappedTextType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Default | `0` | Funziona come MS Excel. |
| Paragraph | `1` | Adatta automaticamente la larghezza con il paragrafo più lungo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitWrappedTextTypeDemo
    {
        public static void AutoFitWrappedTextTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and auto-fitted.\r\n This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted.");
            worksheet.Cells["A5"].PutValue("Another sample text to demonstrate \r\n auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.\r\n Another sample text to demonstrate auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.");

            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            Style style2 = worksheet.Cells["A5"].GetStyle();
            style2.IsTextWrapped = true;
            worksheet.Cells["A5"].SetStyle(style);

            // Crea un intervallo A1:F3
            Range range = worksheet.Cells.CreateRange(0, 0, 3, 6);
            // Unisci le celle
            range.Merge();

            // Crea un intervallo A4:F6
            Range range2 = worksheet.Cells.CreateRange(4, 0, 3, 6);
            // Unisci le celle
            range2.Merge();

            // Crea AutoFitterOptions e imposta AutoFitWrappedTextType
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph;

            // Adatta automaticamente le righe con le opzioni specificate
            worksheet.AutoFitRows(options);

            // Salva la cartella di lavoro
            workbook.Save("AutoFitWrappedTextTypeExample.xlsx");
            workbook.Save("AutoFitWrappedTextTypeExample.pdf");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


