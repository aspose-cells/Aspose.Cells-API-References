---
title: "Protection.AllowSelectingUnlockedCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se l'utente è autorizzato a selezionare le celle non bloccate su un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/allowselectingunlockedcell/
---
## Protection.AllowSelectingUnlockedCell property

Rappresenta se all'utente è consentito selezionare le celle sbloccate su un foglio di lavoro protetto.

```csharp
public bool AllowSelectingUnlockedCell { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingUnlockedCellDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Proteggi il foglio di lavoro con tutte le opzioni di protezione
            Protection protection = worksheet.Protection;
            
            // Imposta AllowSelectingUnlockedCell su true
            protection.AllowSelectingUnlockedCell = true;
            protection.AllowSelectingLockedCell = false;
            
            // Applica la protezione con password
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Verifica l'impostazione
            Console.WriteLine("AllowSelectingUnlockedCell: " + protection.AllowSelectingUnlockedCell);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);

            // Salva la cartella di lavoro
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


