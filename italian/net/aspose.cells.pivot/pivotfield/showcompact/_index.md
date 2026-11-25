---
title: "PivotField.ShowCompact"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se visualizzare le etichette del campo successivo nella stessa colonna nella visualizzazione della Tabella Pivot. Solo per i campi di riga"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/showcompact/
---
## PivotField.ShowCompact property

Indica se visualizzare le etichette del campo successivo nella stessa colonna nella visualizzazione della Tabella Pivot. Solo per i campi di riga.

```csharp
[Obsolete("Use PivotField.ShowInCompactForm instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ShowCompact { get; set; }
```

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.ShowInCompactForm. Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowCompactDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Orange");
            worksheet.Cells["A6"].PutValue("Grape");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["B5"].PutValue(250);
            worksheet.Cells["B6"].PutValue(300);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A7", "A1:B6", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi il campo di riga e configura ShowCompact
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.ShowInOutlineForm = true;
            rowField.ShowCompact = true;
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Calcola e aggiorna la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldShowCompactDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


