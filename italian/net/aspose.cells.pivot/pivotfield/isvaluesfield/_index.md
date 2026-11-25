---
title: "PivotField.IsValuesField"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se questo campo rappresenta il campo valori"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/isvaluesfield/
---
## PivotField.IsValuesField property

Indica se questo campo rappresenta un campo di valori.

```csharp
public bool IsValuesField { get; }
```

### Osservazioni

Funziona solo quando ci sono due o più campi dati nella visualizzazione della tabella pivot.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyIsValuesFieldDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Sales";

            cells["A2"].Value = "Fruit";
            cells["B2"].Value = "Apple";
            cells["C2"].Value = 100;

            cells["A3"].Value = "Fruit";
            cells["B3"].Value = "Orange";
            cells["C3"].Value = 150;

            cells["A4"].Value = "Vegetable";
            cells["B4"].Value = "Carrot";
            cells["C4"].Value = 200;

            cells["A5"].Value = "Vegetable";
            cells["B5"].Value = "Potato";
            cells["C5"].Value = 250;

            // Aggiungi tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            try
            {
                // Ottieni il campo dati (Sales)
                PivotField dataField = pivotTable.DataFields[0];

                // Visualizza il valore della proprietà IsValuesField
                Console.WriteLine("IsValuesField value: " + dataField.IsValuesField);

                // Ottieni un campo riga (Category) per il confronto
                PivotField rowField = pivotTable.RowFields["Category"];
                Console.WriteLine("Row field IsValuesField value: " + rowField.IsValuesField);

                // Calcola i dati e aggiorna
                pivotTable.CalculateData();

                // Salva la cartella di lavoro
                workbook.Save("IsValuesFieldDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


