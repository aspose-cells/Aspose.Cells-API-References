---
title: "PivotField.HideDetail"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Imposta se i dettagli di tutti i PivotItem in un campo pivot sono nascosti. Cioè comprimi/espandi questo campo"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/hidedetail/
---
## PivotField.HideDetail method

Imposta se i dettagli di tutti i PivotItem in un campo pivot sono nascosti. Cioè comprimi/espandi questo campo.

```csharp
[Obsolete("Use PivotItemsCollection.HideAllDetails() and UnhideAllDetails() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideDetail(bool isHiddenDetail)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isHiddenDetail | Booleano | Se nascondere i dettagli del campo pivot. |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare i metodi PivotItemsCollection.HideAllDetails() e UnhideAllDetails(). Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideDetailWithBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Country");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Japan");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("USA");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("UK");
            sheet.Cells["B4"].PutValue(3000);

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Nascondi i dettagli per il primo campo riga
            PivotField rowField = pivotTable.RowFields[0];
            rowField.HideDetail(true);
            
            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("HideDetailDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


