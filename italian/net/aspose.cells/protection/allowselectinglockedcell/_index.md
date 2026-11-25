---
title: "Protection.AllowSelectingLockedCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se all'utente è consentito selezionare celle bloccate su un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/allowselectinglockedcell/
---
## Protection.AllowSelectingLockedCell property

Rappresenta se all'utente è consentito selezionare le celle bloccate su un foglio di lavoro protetto.

```csharp
public bool AllowSelectingLockedCell { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingLockedCellDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta le impostazioni di protezione
            Protection protection = worksheet.Protection;
            
            // Dimostra la proprietà AllowSelectingLockedCell
            protection.AllowSelectingLockedCell = true;
            Console.WriteLine("AllowSelectingLockedCell is set to: " + protection.AllowSelectingLockedCell);

            // Modifica la proprietà e mostra la modifica
            protection.AllowSelectingLockedCell = false;
            Console.WriteLine("AllowSelectingLockedCell is now set to: " + protection.AllowSelectingLockedCell);

            // Proteggi il foglio di lavoro con password
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

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


