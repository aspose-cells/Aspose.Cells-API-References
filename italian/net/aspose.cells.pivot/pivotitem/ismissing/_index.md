---
title: "PivotItem.IsMissing"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotItem. Indica se l'elemento è stato rimosso dalla fonte dati"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/ismissing/
---
## PivotItem.IsMissing property

Indica se l'elemento è stato rimosso dalla fonte dati.

```csharp
public bool IsMissing { get; }
```

### Osservazioni

True indica che questo valore è stato rimosso dalla fonte dati.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsMissingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Crea una tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiorna i dati della tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Ottieni il primo elemento pivot nel primo campo di riga
            PivotField rowField = pivotTable.RowFields[0];
            PivotItem pivotItem = rowField.PivotItems[0];

            // Visualizza il valore della proprietà IsMissing
            Console.WriteLine("IsMissing value for '{0}': {1}", pivotItem.Name, pivotItem.IsMissing);

            // Crea uno scenario in cui un elemento potrebbe mancare
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B5"].PutValue(4000);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Verifica se l'elemento pivot originale è ora mancante
            Console.WriteLine("After data change - IsMissing value for '{0}': {1}", 
                pivotItem.Name, pivotItem.IsMissing);

            // Salva la cartella di lavoro
            workbook.Save("PivotItemIsMissingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


