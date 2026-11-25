---
title: "Cells.IsRowHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Verifica se una riga all'indice specificato è nascosta"
type: docs
url: /it/net/aspose.cells/cells/isrowhidden/
---
## Cells.IsRowHidden method

Verifica se una riga all'indice specificato è nascosta.

```csharp
public bool IsRowHidden(int rowIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | indice della riga |

### Valore di ritorno

vero se la riga è nascosta

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsRowHiddenWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Dati di esempio
            cells[1, 0].PutValue("US");
            cells[2, 0].PutValue("UK");
            cells[3, 0].PutValue("India");
            cells[4, 0].PutValue("UK");
            cells[5, 0].PutValue("India");
            cells[6, 0].PutValue("US");
            
            // Applica filtro
            AutoFilter af = sheet.AutoFilter;
            af.Range = "A1:A1";
            af.Filter(0, "India");
            af.Refresh();
            
            // Verifica visibilità della riga
            Console.WriteLine("Row Visibility Check:");
            for (int i = 1; i < 7; i++)
            {
                Console.WriteLine($"Row {i} hidden: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


