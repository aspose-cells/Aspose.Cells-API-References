---
title: "Protection.AllowDeletingColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se l'eliminazione di colonne è consentita su un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/allowdeletingcolumn/
---
## Protection.AllowDeletingColumn property

Rappresenta se l'eliminazione delle colonne è consentita su un foglio di lavoro protetto.

```csharp
public bool AllowDeletingColumn { get; set; }
```

### Osservazioni

Le colonne contenenti le celle da eliminare devono essere sbloccate quando il foglio è protetto, e l'opzione "Seleziona celle sbloccate" deve essere abilitata.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Abilita la protezione del foglio di lavoro
            Protection protection = worksheet.Protection;
            protection.AllowDeletingColumn = true;
            worksheet.Protect(ProtectionType.All);

            // Verifica l'impostazione
            Console.WriteLine("AllowDeletingColumn: " + protection.AllowDeletingColumn);

            // Prova a eliminare una colonna (dovrebbe funzionare poiché AllowDeletingColumn è true)
            worksheet.Cells.DeleteColumn(0);
            Console.WriteLine("Column deleted successfully");

            // Disabilita l'eliminazione di colonne
            protection.AllowDeletingColumn = false;

            // Prova a eliminare un'altra colonna (dovrebbe fallire)
            try
            {
                worksheet.Cells.DeleteColumn(1);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Failed to delete column: " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


