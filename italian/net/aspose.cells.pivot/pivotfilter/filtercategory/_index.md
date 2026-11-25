---
title: "PivotFilter.FilterCategory"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFilter. Ottiene la categoria di questo filtro"
type: docs
url: /it/net/aspose.cells.pivot/pivotfilter/filtercategory/
---
## PivotFilter.FilterCategory property

Ottiene la categoria di questo filtro.

```csharp
public FilterCategory FilterCategory { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterPropertyFilterCategoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea dati di esempio per la tabella pivot
                worksheet.Cells["A1"].Value = "Category";
                worksheet.Cells["A2"].Value = "A";
                worksheet.Cells["A3"].Value = "B";
                worksheet.Cells["A4"].Value = "A";
                worksheet.Cells["B1"].Value = "Value";
                worksheet.Cells["B2"].Value = 100;
                worksheet.Cells["B3"].Value = 200;
                worksheet.Cells["B4"].Value = 300;

                // Crea tabella pivot
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                
                // Aggiungi il campo riga utilizzando il metodo API corretto
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                
                // Aggiungi il campo dati utilizzando il metodo API corretto
                int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                PivotField dataField = pivotTable.DataFields[dataFieldIndex];
                dataField.Function = ConsolidationFunction.Sum;
                dataField.DisplayName = "Total";

                // Aggiungi un filtro di didascalia al campo Categoria
                int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
                PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];

                // Visualizza il valore della proprietà FilterCategory
                Console.WriteLine("FilterCategory value: " + pivotFilter.FilterCategory);

                workbook.Save("FilterCategoryDemo.xlsx");
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

* enum [FilterCategory](../../../aspose.cells/filtercategory/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


