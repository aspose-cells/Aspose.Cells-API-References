---
title: "PivotTable.ShowDetail"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Mostra il dettaglio di un elemento nella regione dati in una nuova Table"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showdetail/
---
## PivotTable.ShowDetail method

Mostra il dettaglio di un elemento nella regione dati in una nuova tabella.

```csharp
public void ShowDetail(int rowOffset, int columnOffset, bool newSheet, int destRow, int destColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowOffset | Int32 | Offset alla prima riga di dati nella regione dati. |
| columnOffset | Int32 | Offset alla prima colonna di dati nella regione dati. |
| newSheet | Booleano | Mostra il dettaglio in un nuovo foglio di lavoro. |
| destRow | Int32 | La riga di destinazione. |
| destColumn | Int32 | La colonna di destinazione. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowDetailWithInt32Int32BooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Sport");
            worksheet.Cells["A2"].PutValue("Tennis");
            worksheet.Cells["A3"].PutValue("Basketball");
            worksheet.Cells["A4"].PutValue("Tennis");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(80);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(85);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Sport");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Score");

            // Mostra il dettaglio per una cella specifica
            pivotTable.ShowDetail(1, 0, true, 0, 0);

            // Salva la cartella di lavoro
            workbook.Save("PivotTableShowDetailExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


