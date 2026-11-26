---
title: "PivotField.IsAscendSort"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si los elementos de este campo dinámico se ordenan automáticamente de forma ascendente"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/isascendsort/
---
## PivotField.IsAscendSort property

Indica si los elementos de este campo dinámico están ordenados automáticamente de forma ascendente.

```csharp
[Obsolete("Use PivotField.SortSetting.SortType property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAscendSort { get; set; }
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
    public class PivotFieldPropertyIsAscendSortDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["A2"].Value = "B";
            sheet.Cells["A3"].Value = "C";
            sheet.Cells["A4"].Value = "A";
            sheet.Cells["B2"].Value = 150;
            sheet.Cells["B3"].Value = 300;
            sheet.Cells["B4"].Value = 200;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Configurar ordenación
            PivotField sortField = pivotTable.RowFields[0];
            sortField.IsAutoSort = true;
            sortField.IsAscendSort = false; // Demonstrate descending sort
            sortField.AutoSortField = 0; // Sort by first data field
            
            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldIsAscendSortDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


