---
title: "PivotItem.IsCalculatedItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotItem. Indica se questo elemento pivot è un elemento di formula calcolata"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/iscalculateditem/
---
## PivotItem.IsCalculatedItem property

Indica se questo elemento pivot è un elemento di formula calcolata.

```csharp
public bool IsCalculatedItem { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsCalculatedItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 15;

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Calcola i dati della tabella pivot
            pivotTable.CalculateData();

            // Ottieni il primo elemento pivot dal primo campo pivot
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItem pivotItem = pivotField.PivotItems[0];

            // Visualizza il valore della proprietà IsCalculatedItem
            Console.WriteLine("IsCalculatedItem value: " + pivotItem.IsCalculatedItem);

            // Verifica se l'elemento pivot è un elemento calcolato
            if (pivotItem.IsCalculatedItem)
            {
                Console.WriteLine("This pivot item is a calculated formula item.");
                Console.WriteLine("Formula: " + pivotItem.GetFormula());
            }
            else
            {
                Console.WriteLine("This pivot item is not a calculated formula item.");
            }

            // Salva la cartella di lavoro
            workbook.Save("PivotItemPropertyIsCalculatedItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


