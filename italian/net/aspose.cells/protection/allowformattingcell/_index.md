---
title: "Protection.AllowFormattingCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se la formattazione delle celle è consentita su un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/allowformattingcell/
---
## Protection.AllowFormattingCell property

Rappresenta se la formattazione delle celle è consentita su un foglio di lavoro protetto.

```csharp
public bool AllowFormattingCell { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingCellDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Abilita la protezione del foglio di lavoro
            Protection protection = worksheet.Protection;
            
            // Imposta varie proprietà di protezione usando un flag
            int flag = 0x40; // Only AllowFormattingCell flag is set
            protection.AllowFormattingCell = (flag & 0x40) != 0;

            // Verifica l'impostazione
            Console.WriteLine("AllowFormattingCell is set to: " + protection.AllowFormattingCell);

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


