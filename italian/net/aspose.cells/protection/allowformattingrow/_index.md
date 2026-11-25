---
title: "Protection.AllowFormattingRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se la formattazione delle righe è consentita su un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/allowformattingrow/
---
## Protection.AllowFormattingRow property

Rappresenta se la formattazione delle righe è consentita su un foglio di lavoro protetto

```csharp
public bool AllowFormattingRow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Abilita la protezione del foglio di lavoro
            worksheet.Protect(ProtectionType.All);

            // Accedi alle impostazioni di protezione
            Protection protection = worksheet.Protection;

            // Consenti la formattazione delle righe mantenendo le altre protezioni
            protection.AllowFormattingRow = true;

            // Salva la cartella di lavoro
            workbook.Save("Protection_AllowFormattingRow.xlsx");
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


