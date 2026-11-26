---
title: "PivotField.ShowCompact"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si se deben mostrar las etiquetas del siguiente campo en la misma columna en la vista de tabla dinámica. Solo para campos de fila"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/showcompact/
---
## PivotField.ShowCompact property

Indica si se deben mostrar las etiquetas del siguiente campo en la misma columna en la vista de tabla dinámica. Solo para campos de fila.

```csharp
[Obsolete("Use PivotField.ShowInCompactForm instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ShowCompact { get; set; }
```

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotField.ShowInCompactForm. Este método será eliminado 12 meses después, a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowCompactDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Orange");
            worksheet.Cells["A6"].PutValue("Grape");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["B5"].PutValue(250);
            worksheet.Cells["B6"].PutValue(300);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A7", "A1:B6", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregue un campo de fila y configure ShowCompact
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.ShowInOutlineForm = true;
            rowField.ShowCompact = true;
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Calcular y actualizar la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldShowCompactDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


