---
title: "PivotFilterCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFilterCollection. Ottiene l'oggetto pivotfilter all'indice specifico"
type: docs
url: /it/net/aspose.cells.pivot/pivotfiltercollection/item/
---
## PivotFilterCollection indexer

Ottiene l'oggetto pivotfilter all'indice specifico.

```csharp
public PivotFilter this[int index] { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi filtro pivot usando il metodo PivotFilterCollection.Add
            pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[0]; // Using Item property via index
            filter.Name = "SampleFilter";
            filter.Value1 = "100";
            
            // Accedi al filtro usando la proprietà Item e visualizza le informazioni
            Console.WriteLine("Filter Name: " + pivotTable.PivotFilters[0].Name);
            Console.WriteLine("Filter Value1: " + pivotTable.PivotFilters[0].Value1);
            Console.WriteLine("Filter Type: " + pivotTable.PivotFilters[0].FilterType);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../../pivotfilter/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


