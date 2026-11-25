---
title: "Cell.ToJson"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Cell metodo. Converti Cell in dati struct JSON"
type: docs
url: /it/net/aspose.cells/cell/tojson/
---
## Cell.ToJson method

Converti [`Cell`](../) in dati struct JSON.

```csharp
public string ToJson()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodToJsonDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta dati di esempio e stili
            cells["A1"].PutValue(100);
            cells["B6"].Formula = "=A1";
            
            // Ottieni la cella e converti in JSON
            Cell cell = cells["B6"];
            string json = cell.ToJson();
            
            // Genera il JSON
            Console.WriteLine("Cell JSON:");
            Console.WriteLine(json);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


