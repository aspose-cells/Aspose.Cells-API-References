---
title: "PivotField.ShowAllItems"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se visualizzare tutti gli elementi nella vista PivotTable anche se non contengono dati di riepilogo. Il valore predefinito è false."
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/showallitems/
---
## PivotField.ShowAllItems property

Indica se visualizzare tutti gli elementi nella vista PivotTable, anche se non contengono dati di riepilogo. Il valore predefinito è false.

```csharp
public bool ShowAllItems { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowAllItemsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Dati di esempio per la tabella pivot
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Product");
            sheet.Cells["C1"].PutValue("Sales");
            
            sheet.Cells["A2"].PutValue("Electronics");
            sheet.Cells["B2"].PutValue("Laptop");
            sheet.Cells["C2"].PutValue(1200);
            
            sheet.Cells["A3"].PutValue("Electronics");
            sheet.Cells["B3"].PutValue("Phone");
            sheet.Cells["C3"].PutValue(800);
            
            sheet.Cells["A4"].PutValue("Furniture");
            sheet.Cells["B4"].PutValue("Chair");
            sheet.Cells["C4"].PutValue(150);

            // Aggiungi tabella pivot
            int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Imposta la proprietà ShowAllItems per il campo riga
            PivotField rowField = pivotTable.RowFields[0];
            rowField.ShowAllItems = true;

            // Calcola i dati e salva
            pivotTable.CalculateData();
            workbook.Save("PivotFieldShowAllItemsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


