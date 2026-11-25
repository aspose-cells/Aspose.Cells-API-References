---
title: "Enum FilterCategory"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.FilterCategory. Rappresenta la categoria del filtro"
type: docs
url: /it/net/aspose.cells/filtercategory/
---
## FilterCategory enumeration

Rappresenta la categoria del filtro.

```csharp
public enum FilterCategory
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessun filtro. |
| Label | `1` | Filtro didascalia. |
| NumberValue | `2` | Filtro valore numerico. |
| Date | `3` | Filtro valore data. |
| Top10 | `4` | Filtro valore Top10. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CellsClassFilterCategoryDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            CreateSampleData(worksheet);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:C7", "H5");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Configura i campi di riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            
            // Configura il campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Aggiungi filtro etichetta ai filtri pivot
            PivotFilter filter = pivotTable.PivotFilters.AddLabelFilter(0, PivotFilterType.CaptionEqual, "East", null);
            
            // Dimostra l'uso di FilterCategory
            Console.WriteLine("Filter Category: " + filter.FilterCategory);
            
            // Visualizza tutte le categorie di filtro nella tabella pivot
            foreach (PivotFilter pivotFilter in pivotTable.PivotFilters)
            {
                Console.WriteLine($"Filter Type: {pivotFilter.FilterType}, Category: {pivotFilter.FilterCategory}");
            }

            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva il risultato
            workbook.Save("FilterCategoryDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Imposta intestazioni dei dati di esempio
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";

            // Aggiungi righe di dati di esempio
            object[,] data = new object[,]
            {
                {"East", "Apples", 5000},
                {"West", "Oranges", 3000},
                {"East", "Bananas", 4000},
                {"North", "Apples", 6000},
                {"South", "Oranges", 2000},
                {"East", "Bananas", 4500},
                {"West", "Apples", 5500}
            };

            int rowCount = data.GetLength(0);
            int colCount = data.GetLength(1);

            for (int i = 0; i < rowCount; i++)
            {
                for (int j = 0; j < colCount; j++)
                {
                    worksheet.Cells[i + 2, j].Value = data[i, j];
                }
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


