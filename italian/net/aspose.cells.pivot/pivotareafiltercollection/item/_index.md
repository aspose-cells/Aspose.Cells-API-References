---
title: "PivotAreaFilterCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotAreaFilterCollection. Ottiene il filtro dall'elenco per indice"
type: docs
url: /it/net/aspose.cells.pivot/pivotareafiltercollection/item/
---
## PivotAreaFilterCollection indexer

Ottiene il filtro dall'elenco per indice.

```csharp
public PivotAreaFilter this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            
            // Aggiungi tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campi alle aree pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Crea formato condizionale
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;
            
            // Crea area pivot e aggiungi filtri
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Value");
            pcf.PivotAreas.Add(pivotArea);
            
            // Dimostra l'uso della proprietà Item
            PivotAreaFilter filter = pivotArea.Filters[0];
            filter.IsSubtotalSet(PivotFieldSubtotalType.Automatic);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotAreaFilterCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotAreaFilter](../../pivotareafilter/)
* class [PivotAreaFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


