---
title: "PivotTable.DisplayNullString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotTable property. Indica se il report PivotTable visualizza una stringa personalizzata se il valore è nullo"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/displaynullstring/
---
## PivotTable.DisplayNullString property

Indica se il report PivotTable visualizza una stringa personalizzata se il valore è null.

```csharp
public bool DisplayNullString { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayNullStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e riempilo con dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue(null);
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(null);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Imposta la proprietà DisplayNullString e la stringa null personalizzata
            pivotTable.DisplayNullString = true;
            pivotTable.NullString = "N/A";
            
            // Calcola i dati e aggiorna la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableDisplayNullStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


