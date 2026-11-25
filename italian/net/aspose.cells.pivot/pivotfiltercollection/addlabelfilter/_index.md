---
title: "PivotFilterCollection.AddLabelFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotFilterCollection. Filtra per didascalie del pivot field di riga o colonna"
type: docs
url: /it/net/aspose.cells.pivot/pivotfiltercollection/addlabelfilter/
---
## PivotFilterCollection.AddLabelFilter method

Filtra per didascalie del campo pivot di riga o colonna.

```csharp
public PivotFilter AddLabelFilter(int baseFieldIndex, PivotFilterType type, string label1, 
    string label2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baseFieldIndex | Int32 | L'indice del campo nella sorgente. |
| type | PivotFilterType | Il tipo di dati di filtraggio. |
| label1 | String | L'etichetta della condizione di filtro |
| label2 | String | L'etichetta superiore della condizione di filtro tra |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddLabelFilterWithInt32PivotFilterTypeStringStriDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Cherry";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

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
                
                // Aggiungi filtro etichetta per mostrare i prodotti che iniziano con "A"
                PivotFilter filter = filters.AddLabelFilter(
                    baseFieldIndex: 0,
                    type: PivotFilterType.CaptionBeginsWith,
                    label1: "A",
                    label2: null
                );

                Console.WriteLine($"Label filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value1: {filter.Value1}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding label filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddLabelFilterDemo.xlsx");
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


