---
title: "PivotField.HideItemDetail"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Imposta se lo specifico PivotItem in un campo pivot è un dettaglio nascosto"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/hideitemdetail/
---
## PivotField.HideItemDetail method

Imposta se lo specifico PivotItem in un campo pivot è un dettaglio nascosto.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItemDetail(int index, bool isHiddenDetail)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | l'indice del pivotItem nel pivotField. |
| isHiddenDetail | Booleano | se il PivotItem specifico è nascosto |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.PivotItems[int].IsDetailHidden. Questo metodo sarà rimosso tra 12 mesi a partire da agosto 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemDetailWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("SampleData.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("East");
            worksheet.Cells["A5"].PutValue("West");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Aggiungi tabella pivot
            int index = worksheet.PivotTables.Add("A1:B5", "H5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campi alle aree
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Nascondi il dettaglio dell'elemento all'indice 2 (East) con isHidden=false
            pivotField.HideItemDetail(2, false);
            
            // Aggiorna e calcola i dati della tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTable_HideItemDetail_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


