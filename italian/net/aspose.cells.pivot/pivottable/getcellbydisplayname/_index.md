---
title: "PivotTable.GetCellByDisplayName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Ottiene l'oggetto Cell per il nome visualizzato di PivotField"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/getcellbydisplayname/
---
## PivotTable.GetCellByDisplayName method

Ottiene l'oggetto [`Cell`](../../../aspose.cells/cell/) per il nome visualizzato di PivotField.

```csharp
public Cell GetCellByDisplayName(string displayName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| displayName | String | il DisplayName di PivotField |

### Valore di ritorno

l'oggetto Cell

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetCellByDisplayNameWithStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Ottieni il nome visualizzato del campo dati
            string displayName = pivotTable.DataFields[0].DisplayName;

            // Usa il metodo GetCellByDisplayName
            Cell cell = pivotTable.GetCellByDisplayName(displayName);

            // Restituisci i risultati
            Console.WriteLine("Display Name: " + displayName);
            Console.WriteLine("Cell Name: " + (cell != null ? cell.Name : "null"));
            Console.WriteLine("Cell Value: " + (cell != null ? cell.Value.ToString() : "null"));

            // Salva la cartella di lavoro
            workbook.Save("PivotTable_GetCellByDisplayName_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../../aspose.cells/cell/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


