---
title: "Cells.GetLastDataRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Ottiene l'indice dell'ultima riga della cella che contiene dati nella colonna specificata"
type: docs
url: /it/net/aspose.cells/cells/getlastdatarow/
---
## Cells.GetLastDataRow method

Restituisce l'indice dell'ultima riga della cella che contiene dati nella colonna specificata.

```csharp
public int GetLastDataRow(int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice colonna. |

### Valore di ritorno

indice dell'ultima riga.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetLastDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            
            // Ottieni l'ultima riga con dati nella colonna A (indice 0)
            int lastRow = worksheet.Cells.GetLastDataRow(0);
            
            // Restituisci il risultato
            Console.WriteLine("Last data row in column A: " + lastRow);
            
            // Inserisci una nuova riga dopo l'ultima riga con dati
            CellArea area = new CellArea();
            area.StartRow = lastRow + 1;
            area.EndRow = lastRow + 1;
            area.StartColumn = 0;
            area.EndColumn = 0;
            worksheet.Cells.InsertRange(area, 1, ShiftType.Down);
            
            // Aggiungi dati alla nuova riga
            worksheet.Cells[lastRow + 2, 0].PutValue("New Data");
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


