---
title: "PivotFilterCollection.AddValueFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotFilterCollection. Filtra per valori del campo pivot dei dati"
type: docs
url: /it/net/aspose.cells.pivot/pivotfiltercollection/addvaluefilter/
---
## PivotFilterCollection.AddValueFilter method

Filtra per valori del campo pivot dei dati.

```csharp
public PivotFilter AddValueFilter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type, 
    double value1, double value2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baseFieldIndex | Int32 | L'indice del campo nella sorgente. |
| valueFieldIndex | Int32 | L'indice del campo valore nella regione dei valori. |
| type | PivotFilterType | Il tipo di dati di filtraggio. |
| value1 | Double | Il valore della condizione di filtro |
| value2 | Double | Il valore superiore della condizione di filtro tra |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddValueFilterWithInt32Int32PivotFilterTypeDoublDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Widget";
            worksheet.Cells["A3"].Value = "Gadget";
            worksheet.Cells["A4"].Value = "Thingy";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["B2"].Value = 15.99;
            worksheet.Cells["B3"].Value = 24.99;
            worksheet.Cells["B4"].Value = 9.99;

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
                
                // Aggiungi filtro valore per mostrare i prodotti con prezzo compreso tra $10 e $20
                PivotFilter filter = filters.AddValueFilter(
                    baseFieldIndex: 0,
                    valueFieldIndex: 1,
                    type: PivotFilterType.ValueBetween,
                    value1: 10.0,
                    value2: 20.0
                );

                Console.WriteLine($"Value filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding value filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddValueFilterDemo.xlsx");
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


