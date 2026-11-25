---
title: "PivotFilterCollection.AddTop10Filter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotFilterCollection. Filtra per valori del campo pivot dei dati"
type: docs
url: /it/net/aspose.cells.pivot/pivotfiltercollection/addtop10filter/
---
## PivotFilterCollection.AddTop10Filter method

Filtra per valori del campo pivot dei dati.

```csharp
public PivotFilter AddTop10Filter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type, 
    bool isTop, int itemCount)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| baseFieldIndex | Int32 | L'indice del campo nella sorgente. |
| valueFieldIndex | Int32 | L'indice del campo dati nella regione dei dati. |
| type | PivotFilterType | Il tipo di filtraggio dei dati. Può essere solo Count, Sum e Percent. |
| isTop | Booleano | Indica se il filtro è dall'alto o dal basso |
| itemCount | Int32 | Il conteggio degli elementi |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddTop10FilterWithInt32Int32PivotFilterTypeBooleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Dairy";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 80;
            worksheet.Cells["B4"].Value = 120;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Ottieni la collezione di filtri pivot
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // Aggiungi filtro Top10 - mostra i primi 2 elementi per vendite
                PivotFilter filter = filters.AddTop10Filter(
                    baseFieldIndex: 0,          // Category field
                    valueFieldIndex: 1,          // Sales field
                    type: PivotFilterType.Count, // Filter type
                    isTop: true,                 // Show top items
                    itemCount: 2                 // Number of items to show
                );

                Console.WriteLine($"Top10 filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding Top10 filter: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFilterCollectionMethodAddTop10FilterDemo.xlsx");
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


