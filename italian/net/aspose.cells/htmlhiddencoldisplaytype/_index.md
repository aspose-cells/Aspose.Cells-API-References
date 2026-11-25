---
title: "Enum HtmlHiddenColDisplayType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.HtmlHiddenColDisplayType. Rappresenta due tipi di visualizzazione delle colonne nascoste in HTML"
type: docs
url: /it/net/aspose.cells/htmlhiddencoldisplaytype/
---
## HtmlHiddenColDisplayType enumeration

Rappresenta due tipi di visualizzazione delle colonne nascoste in HTML.

```csharp
public enum HtmlHiddenColDisplayType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Hidden | `0` | Nascondi le colonne nascoste nella pagina HTML. |
| Remove | `1` | Rimuovi le colonne nascoste nella pagina HTML. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenColDisplayTypeDemo
    {
        public static void HtmlHiddenColDisplayTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Nascondi la seconda colonna
            worksheet.Cells.HideColumn(1);

            // Crea HtmlSaveOptions e imposta HiddenColDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;

            // Salva la cartella di lavoro in formato HTML
            workbook.Save("HtmlHiddenColDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden columns removed.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


