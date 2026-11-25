---
title: "PivotField.AddCalculatedItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Aggiunge un elemento formula calcolata al campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/addcalculateditem/
---
## PivotField.AddCalculatedItem method

Aggiunge un elemento formula calcolata al campo pivot.

```csharp
public void AddCalculatedItem(string name, string formula)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome dell'elemento. |
| formula | String | La formula dell'elemento pivot. |

### Osservazioni

Supporta solo l'aggiunta di elementi calcolati al campo Riga/Colonna.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodAddCalculatedItemWithStringStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["A2"].Value = "grape";
            sheet.Cells["A3"].Value = "kiwi";
            sheet.Cells["A4"].Value = "grape";
            sheet.Cells["A5"].Value = "kiwi";
            
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 50;
            sheet.Cells["B3"].Value = 70;
            sheet.Cells["B4"].Value = 30;
            sheet.Cells["B5"].Value = 20;

            // Crea una tabella pivot con i parametri corretti
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ottieni il campo pivot e aggiungi l'elemento calcolato
            PivotField fruitField = pivotTable.RowFields[0];
            fruitField.AddCalculatedItem("grape_kiwi_total", "=grape + kiwi");
            
            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldAddCalculatedItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


