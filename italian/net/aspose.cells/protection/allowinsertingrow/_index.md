---
title: "Protection.AllowInsertingRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se l'inserimento di righe è consentito su un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/allowinsertingrow/
---
## Protection.AllowInsertingRow property

Rappresenta se l'inserimento delle righe è consentito su un foglio di lavoro protetto

```csharp
public bool AllowInsertingRow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alle impostazioni di protezione
            Protection protection = worksheet.Protection;

            // Abilita l'inserimento di righe durante la protezione
            protection.AllowInsertingRow = true;
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Prova a inserire una riga (dovrebbe funzionare poiché AllowInsertingRow è true)
            worksheet.Cells.InsertRow(0);

            // Salva la cartella di lavoro
            workbook.Save("AllowInsertingRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


