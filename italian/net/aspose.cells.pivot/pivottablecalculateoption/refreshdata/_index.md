---
title: "PivotTableCalculateOption.RefreshData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotTableCalculateOption property. Indica se aggiornare la fonte dati della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottablecalculateoption/refreshdata/
---
## PivotTableCalculateOption.RefreshData property

Indica se la fonte dati della tabella pivot viene aggiornata.

```csharp
public bool RefreshData { get; set; }
```

### Osservazioni

Se è vero, aggiorna la cache pivot dalla fonte dati, quindi calcola tutte le tabelle pivot basate sulla stessa cache pivot.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyRefreshDataDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Configura dati di esempio per la tabella pivot
            var cells = sheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("A");
            cells["B2"].PutValue(100);
            cells["A3"].PutValue("B");
            cells["B3"].PutValue(200);
            cells["A4"].PutValue("C");
            cells["B4"].PutValue(300);

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Modifica i dati di origine
            cells["B2"].PutValue(150); // Change value from 100 to 150

            // Calcola la tabella pivot con l'opzione RefreshData
            PivotTableCalculateOption options = new PivotTableCalculateOption();
            options.RefreshData = true;
            pivotTable.CalculateData(options);

            // Restituisci il valore aggiornato della tabella pivot
            Console.WriteLine("Updated Pivot Table Value: " + cells["F5"].StringValue);
        }
    }
}
```

### Vedi anche

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


