---
title: "Protection.AllowInsertingColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se l'inserimento di colonne è consentito su un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/allowinsertingcolumn/
---
## Protection.AllowInsertingColumn property

Rappresenta se l'inserimento delle colonne è consentito su un foglio di lavoro protetto

```csharp
public bool AllowInsertingColumn { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni le impostazioni di protezione
            Protection protection = worksheet.Protection;

            // Imposta AllowInsertingColumn su true
            protection.AllowInsertingColumn = true;

            // Verifica l'impostazione
            Console.WriteLine("AllowInsertingColumn is set to: " + protection.AllowInsertingColumn);

            // Proteggi il foglio di lavoro con password (usando il metodo Workbook.Protect)
            workbook.Protect(ProtectionType.All, "password123");
            protection.AllowInsertingColumn = true; // Explicitly set again to demonstrate

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


