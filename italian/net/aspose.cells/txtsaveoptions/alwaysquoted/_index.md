---
title: "TxtSaveOptions.AlwaysQuoted"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtSaveOptions. Indica se aggiungere sempre  per ogni campo. Se true tutti i valori saranno racchiusi tra virgolette. Se false i valori saranno racchiusi tra virgolette solo quando necessario, ad esempio quando i valori contengono caratteri speciali come   n o il carattere separatore. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/alwaysquoted/
---
## TxtSaveOptions.AlwaysQuoted property

Indica se aggiungere sempre '\\"' per ogni campo. Se true tutti i valori saranno racchiusi tra virgolette; se false i valori saranno racchiusi tra virgolette solo quando necessario (ad esempio, quando i valori contengono caratteri speciali come '\\"', '\\n' o il carattere separatore). Il valore predefinito è false.

```csharp
[Obsolete("Use QuoteType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AlwaysQuoted { get; set; }
```

### Osservazioni

NOTE: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà QuoteType. Questa proprietà sarà rimossa tra 12 mesi a partire da agosto 2012. Aspose si scusa per qualsiasi inconveniente possa aver riscontrato.

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);

            // Crea TxtSaveOptions con AlwaysQuoted impostato su true
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                AlwaysQuoted = true,
                QuoteType = TxtValueQuoteType.Always
            };

            // Salva con virgolette attorno a tutti i valori
            workbook.Save("AlwaysQuoted_True.txt", saveOptions);

            // Modifica su false e salva nuovamente
            saveOptions.AlwaysQuoted = false;
            workbook.Save("AlwaysQuoted_False.txt", saveOptions);

            Console.WriteLine("Files saved with different AlwaysQuoted settings.");
        }
    }
}
```

### Vedi anche

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


