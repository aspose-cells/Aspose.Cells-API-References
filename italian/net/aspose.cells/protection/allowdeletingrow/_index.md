---
title: "Protection.AllowDeletingRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se l\\'eliminazione delle righe è consentita in un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/allowdeletingrow/
---
## Protection.AllowDeletingRow property

Rappresenta se l'eliminazione delle righe è consentita su un foglio di lavoro protetto.

```csharp
public bool AllowDeletingRow { get; set; }
```

### Osservazioni

Le righe contenenti le celle da eliminare devono essere sbloccate quando il foglio è protetto, e l'opzione "Seleziona celle sbloccate" deve essere abilitata.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Imposta le impostazioni di protezione
            Protection protection = sheet.Protection;
            protection.AllowDeletingRow = true;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingColumn = true;

            // Proteggi il foglio di lavoro
            sheet.Protect(ProtectionType.All);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");

            // Carica la cartella di lavoro salvata per verificare le impostazioni
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            // Verifica AllowDeletingRow e altre proprietà
            Console.WriteLine("AllowDeletingRow: " + loadedSheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowSorting: " + loadedSheet.Protection.AllowSorting);
            Console.WriteLine("AllowFiltering: " + loadedSheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingColumn: " + loadedSheet.Protection.AllowFormattingColumn);
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


