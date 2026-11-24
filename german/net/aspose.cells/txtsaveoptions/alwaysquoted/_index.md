---
title: "TxtSaveOptions.AlwaysQuoted"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Eigenschaft. Gibt an, ob für jedes Feld immer ein Anführungszeichen hinzugefügt wird. Wenn true, werden alle Werte in Anführungszeichen gesetzt; wenn false, werden Werte nur bei Bedarf in Anführungszeichen gesetzt, zum Beispiel wenn Werte Sonderzeichen wie   n oder das Trennzeichen enthalten. Standard ist false."
type: docs
url: /de/net/aspose.cells/txtsaveoptions/alwaysquoted/
---
## TxtSaveOptions.AlwaysQuoted property

Gibt an, ob für jedes Feld immer ein '\"' hinzugefügt wird. Wenn true, werden alle Werte in Anführungszeichen gesetzt; wenn false, werden Werte nur bei Bedarf in Anführungszeichen gesetzt (zum Beispiel, wenn Werte Sonderzeichen wie '\"', '\\n' oder das Trennzeichen enthalten). Standard ist false.

```csharp
[Obsolete("Use QuoteType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AlwaysQuoted { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die QuoteType‑Eigenschaft. Diese Eigenschaft wird 12 Monate nach August 2012 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyAlwaysQuotedDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);

            // Erstellen Sie TxtSaveOptions mit AlwaysQuoted auf true gesetzt
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                AlwaysQuoted = true,
                QuoteType = TxtValueQuoteType.Always
            };

            // Speichern mit Anführungszeichen um alle Werte
            workbook.Save("AlwaysQuoted_True.txt", saveOptions);

            // Auf false ändern und erneut speichern
            saveOptions.AlwaysQuoted = false;
            workbook.Save("AlwaysQuoted_False.txt", saveOptions);

            Console.WriteLine("Files saved with different AlwaysQuoted settings.");
        }
    }
}
```

### Siehe auch

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


