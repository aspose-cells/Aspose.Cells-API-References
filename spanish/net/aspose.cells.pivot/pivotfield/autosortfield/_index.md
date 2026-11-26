---
title: "PivotField.AutoSortField"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Representa el índice del campo que se ordena automáticamente. 1 significa el propio PivotField; otros valores indican la posición de los campos de datos."
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/autosortfield/
---
## PivotField.AutoSortField property

Representa el índice del campo que se ordena automáticamente. -1 significa el propio PivotField; otros valores indican la posición de los campos de datos.

```csharp
[Obsolete("Use PivotField.SortSetting.SortBy property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoSortField { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.SortSetting.SortBy o el método PivotField.SortBy(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoSortFieldDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Branch";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "North";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "South";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "East";
            cells["B4"].Value = 800;
            cells["A5"].Value = "West";
            cells["B5"].Value = 1200;

            // Agregar tabla dinámica
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Branch");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtener el campo de pivote
            PivotField pivotField = pivotTable.RowFields["Branch"];

            // Configurar orden automático
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;
            pivotField.AutoSortField = 0; // Sort by first data field (Sales)

            // Calcular datos y actualizar
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldAutoSortDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


