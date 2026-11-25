---
title: "Enum HtmlHiddenRowDisplayType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.HtmlHiddenRowDisplayType enum. Rappresenta due tipi di visualizzazione delle righe nascoste in HTML"
type: docs
url: /it/net/aspose.cells/htmlhiddenrowdisplaytype/
---
## HtmlHiddenRowDisplayType enumeration

Rappresenta due tipi di visualizzazione delle righe nascoste in HTML.

```csharp
public enum HtmlHiddenRowDisplayType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Hidden | `0` | Nascondi le righe nascoste nella pagina HTML. |
| Remove | `1` | Rimuovi le righe nascoste nella pagina HTML. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenRowDisplayTypeDemo
    {
        public static void HtmlHiddenRowDisplayTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Another Visible Row");

            // Nascondi la seconda riga
            worksheet.Cells.HideRow(1);

            // Crea HtmlSaveOptions e imposta HiddenRowDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden; // or HtmlHiddenRowDisplayType.Remove

            // Salva la cartella di lavoro in formato HTML
            workbook.Save("HtmlHiddenRowDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden row display type.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


