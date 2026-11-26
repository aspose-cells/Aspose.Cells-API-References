---
title: "PivotTable.DataField"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Obtiene un objeto PivotField que representa todos los campos de datos en una tabla dinámica. Solo de lectura. Solo se crea cuando hay dos o más campos de datos en la región de Datos. Por defecto está en la región de filas. Puede arrastrarlo a la región de filas/columnas con el método PivotTable.AddFieldToArea."
type: docs
url: /es/net/aspose.cells.pivot/pivottable/datafield/
---
## PivotTable.DataField property

Obtiene un objeto [`PivotField`](../../pivotfield/) que representa todos los campos de datos en una tabla dinámica. Solo de lectura. Solo se crea cuando hay dos o más campos de datos en la región de Datos. Por defecto está en la región de filas. Puede arrastrarlo a la región de filas/columnas con el método PivotTable.AddFieldToArea().

```csharp
[Obsolete("Use PivotTable.ValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotField DataField { get; }
```

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotTable.ValuesField. Este método será eliminado 12 meses después, a partir de octubre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Acceder y modificar las propiedades de DataField
            // La posición es solo de lectura, así que demostraremos otras propiedades
            pivotTable.DataField.DisplayName = "Total Sales";
            pivotTable.DataField.NumberFormat = "#,##0";
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableDataFieldDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


