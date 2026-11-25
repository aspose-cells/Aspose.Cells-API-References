---
title: "Cells.DeleteRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Elimina un range di celle e sposta le celle secondo l'opzione di spostamento"
type: docs
url: /it/net/aspose.cells/cells/deleterange/
---
## Cells.DeleteRange method

Elimina un intervallo di celle e sposta le celle secondo l'opzione di spostamento.

```csharp
public void DeleteRange(int startRow, int startColumn, int endRow, int endColumn, 
    ShiftType shiftType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Indice della riga iniziale. |
| startColumn | Int32 | Indice della colonna iniziale. |
| endRow | Int32 | Indice della riga finale. |
| endColumn | Int32 | Indice della colonna finale. |
| shiftType | ShiftType | Opzione sposta celle. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRangeWithInt32Int32Int32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Popola alcuni dati di esempio
            sheet.Cells["A1"].PutValue("A1");
            sheet.Cells["B1"].PutValue("B1");
            sheet.Cells["C1"].PutValue("C1");
            sheet.Cells["A2"].PutValue("A2");
            sheet.Cells["B2"].PutValue("B2");
            sheet.Cells["C2"].PutValue("C2");

            // Elimina il range e sposta a sinistra
            sheet.Cells.DeleteRange(0, 1, 1, 2, ShiftType.Left);

            // Salva la cartella di lavoro
            workbook.Save("DeleteRangeExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


