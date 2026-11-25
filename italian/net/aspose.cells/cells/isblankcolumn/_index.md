---
title: "Cells.IsBlankColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Verifica se la colonna specificata è vuota e non contiene dati"
type: docs
url: /it/net/aspose.cells/cells/isblankcolumn/
---
## Cells.IsBlankColumn method

Verifica se la colonna specificata è vuota (non contiene alcun dato).

```csharp
public bool IsBlankColumn(int columnIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | l'indice della colonna |

### Valore di ritorno

vero se la colonna specificata non contiene dati

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsBlankColumnWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Verifica se la colonna 2 è vuota (dovrebbe essere vero per un nuovo foglio di lavoro)
            Console.WriteLine("Is column 2 blank? " + worksheet.Cells.IsBlankColumn(1));

            // Aggiungi dati alla colonna 2
            worksheet.Cells["B1"].PutValue("Test Data");

            // Verifica di nuovo (dovrebbe ora essere falso)
            Console.WriteLine("Is column 2 blank after adding data? " + worksheet.Cells.IsBlankColumn(1));

            // Crea un altro foglio di lavoro con colonne completamente vuote
            Worksheet worksheet2 = workbook.Worksheets.Add("BlankSheet");

            // Verifica una colonna nel foglio di lavoro vuoto (dovrebbe essere vero)
            Console.WriteLine("Is column 3 blank in new sheet? " + worksheet2.Cells.IsBlankColumn(2));
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


