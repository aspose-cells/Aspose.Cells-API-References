---
title: "PivotFilterCollection.AddDateFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotFilterCollection. Filtra per impostazione data del campo pivot di riga o colonna"
type: docs
url: /it/net/aspose.cells.pivot/pivotfiltercollection/adddatefilter/
---
## PivotFilterCollection.AddDateFilter method

Filtra per impostazione della data del campo pivot di riga o colonna.

```csharp
public PivotFilter AddDateFilter(int baseFieldIndex, PivotFilterType type, DateTime dateTime1, 
    DateTime dateTime2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baseFieldIndex | Int32 | L'indice del campo nella sorgente. |
| type | PivotFilterType | Il tipo di dati di filtraggio. |
| dateTime1 | DateTime | L'etichetta data della condizione di filtro |
| dateTime2 | DateTime | L'etichetta data superiore della condizione di filtro tra |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddDateFilterWithInt32PivotFilterTypeDateTimeDaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con date
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // Aggiungi filtro data per mostrare le date tra 1 gennaio e 31 marzo 2023
                PivotFilter filter = filters.AddDateFilter(
                    baseFieldIndex: 0,
                    type: PivotFilterType.DateBetween,
                    dateTime1: new DateTime(2023, 1, 1),
                    dateTime2: new DateTime(2023, 3, 31)
                );

                Console.WriteLine($"Date filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, UseWholeDay: {filter.UseWholeDay}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding date filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddDateFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


