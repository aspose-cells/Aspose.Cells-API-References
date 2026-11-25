---
title: "PivotTable.IsMultipleFieldFilters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Specifica un valore booleano che indica se i campi di una PivotTable possono avere più filtri impostati su di essi"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/ismultiplefieldfilters/
---
## PivotTable.IsMultipleFieldFilters property

Specifica un valore booleano che indica se i campi di una PivotTable possono avere più filtri impostati su di essi.

```csharp
[Obsolete("Use PivotTable.AllowMultipleFiltersPerField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsMultipleFieldFilters { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà PivotTable.AllowMultipleFiltersPerField. Questo metodo sarà rimosso 12 mesi dopo a partire da dicembre 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyIsMultipleFieldFiltersDemo
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
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("Fruit");
            worksheet.Cells["B3"].PutValue("Fruit");
            worksheet.Cells["B4"].PutValue("Fruit");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Crea una tabella pivot
            int index = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visualizza il valore corrente di IsMultipleFieldFilters
            Console.WriteLine("Current IsMultipleFieldFilters value: " + pivotTable.IsMultipleFieldFilters);

            // Imposta IsMultipleFieldFilters su true per consentire più filtri per campo
            pivotTable.IsMultipleFieldFilters = true;
            Console.WriteLine("IsMultipleFieldFilters set to: " + pivotTable.IsMultipleFieldFilters);

            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTablePropertyIsMultipleFieldFiltersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


