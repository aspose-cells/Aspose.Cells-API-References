---
title: "PivotField.IsAutoSort"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PivotField property. Indica si los elementos de este campo de tabla dinámica se ordenan automáticamente"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/isautosort/
---
## PivotField.IsAutoSort property

Indica si los elementos de este campo de tabla dinámica se ordenan automáticamente.

```csharp
[Obsolete("Use PivotField.SortSetting.SortType property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAutoSort { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.SortSetting.SortType o el método PivotField.SortBy(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoSortDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            cells["A5"].Value = "Blueberry";
            cells["B5"].Value = 15;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campo de fila y establecer orden automático
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.IsAutoSort = true;
            rowField.AutoSortField = 1; // Sort by Quantity (column B)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldIsAutoSortDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


