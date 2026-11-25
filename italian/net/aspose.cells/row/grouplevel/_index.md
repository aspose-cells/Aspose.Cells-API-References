---
title: "Row.GroupLevel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Row. Ottiene il livello di raggruppamento della riga"
type: docs
url: /it/net/aspose.cells/row/grouplevel/
---
## Row.GroupLevel property

Ottiene il livello di gruppo della riga.

```csharp
public byte GroupLevel { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Raggruppa le righe 4-6 (nascosto = false)
            worksheet.Cells.GroupRows(3, 5, false);

            // Accedi al livello di raggruppamento della riga 4
            int groupLevel = worksheet.Cells.Rows[3].GroupLevel;
            Console.WriteLine("Group level of row 4: " + groupLevel);

            // Separa le righe dal raggruppamento
            worksheet.Cells.UngroupRows(3, 5);
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


