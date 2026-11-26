---
title: "PivotFilterCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotFilterCollection. Agrega un objeto PivotFilter al tipo específico"
type: docs
url: /es/net/aspose.cells.pivot/pivotfiltercollection/add/
---
## PivotFilterCollection.Add method

Agrega un objeto PivotFilter al tipo específico

```csharp
[Obsolete("Use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods,instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int fieldIndex, PivotFilterType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | el índice del PivotField |
| type | PivotFilterType | el tipo de PivotFilter |

### Valor de retorno

el índice del objeto PivotFilter en esta PivotFilterCollection.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice los métodos PivotFilterCollection.AddValueFilter(), AddTop10Filter(), AddLabelFilter() y AddDateFilter(). Este método será eliminado 12 meses después, a partir de noviembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

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

            // Datos de ejemplo
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

            // Crear tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");

            // Agregar filtro pivot
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

### Ver también

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


