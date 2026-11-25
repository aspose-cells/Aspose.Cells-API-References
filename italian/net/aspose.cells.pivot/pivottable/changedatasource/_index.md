---
title: "PivotTable.ChangeDataSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Cambia la fonte dati della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/changedatasource/
---
## PivotTable.ChangeDataSource method

Modifica l'origine dati della tabella pivot.

```csharp
public void ChangeDataSource(string[] source)
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot; // Added this using directive
    using System;

    public class PivotTableMethodChangeDataSourceWithStringDemo
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
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Prepara una nuova fonte dati
            string[] newDataSource = new string[] { "C1:D4", "Sheet1" };

            try
            {
                // Cambia la fonte dati della tabella pivot
                pivotTable.ChangeDataSource(newDataSource);

                // Aggiorna la tabella pivot per applicare le modifiche
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable data source changed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing pivot table data source: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("PivotTableChangeDataSourceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


