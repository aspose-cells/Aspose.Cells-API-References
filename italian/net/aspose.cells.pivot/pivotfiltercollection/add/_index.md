---
title: "PivotFilterCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotFilterCollection. Aggiunge un oggetto PivotFilter al tipo specifico"
type: docs
url: /it/net/aspose.cells.pivot/pivotfiltercollection/add/
---
## PivotFilterCollection.Add method

Aggiunge un oggetto PivotFilter al tipo specifico

```csharp
[Obsolete("Use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods,instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int fieldIndex, PivotFilterType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | l'indice del PivotField |
| type | PivotFilterType | il tipo PivotFilter |

### Valore di ritorno

l'indice dell'oggetto PivotFilter in questa PivotFilterCollection.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare i metodi PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() e AddDateFilter(). Questo metodo sarà rimosso tra 12 mesi a partire da novembre 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterCollectionMethodAddWithInt32PivotFilterTypeDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Dati di esempio
            cells["A1"].Value = "Category";
            cells["A2"].Value = "A";
            cells["A3"].Value = "B";
            cells["A4"].Value = "A";
            cells["A5"].Value = "B";
            
            cells["B1"].Value = "Value";
            cells["B2"].Value = 10;
            cells["B3"].Value = 20;
            cells["B4"].Value = 30;
            cells["B5"].Value = 40;

            // Crea tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");

            // Aggiungi filtro pivot
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            pivot.RefreshData();
            pivot.CalculateData();

            book.Save("PivotFilterDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


