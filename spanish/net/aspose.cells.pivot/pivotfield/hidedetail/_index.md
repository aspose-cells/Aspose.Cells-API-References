---
title: "PivotField.HideDetail"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PivotField method. Establece si el detalle de todos los PivotItems en un campo dinámico está oculto. Es decir, colapsar/expandir este campo"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/hidedetail/
---
## PivotField.HideDetail method

Establece si el detalle de todos los PivotItems en un campo dinámico está oculto. Es decir, colapsar/expandir este campo.

```csharp
[Obsolete("Use PivotItemsCollection.HideAllDetails() and UnhideAllDetails() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideDetail(bool isHiddenDetail)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isHiddenDetail | Booleano | Si oculta el detalle del campo de tabla dinámica. |

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use los métodos PivotItemsCollection.HideAllDetails() y UnhideAllDetails(). Este método será eliminado 12 meses después, a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideDetailWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Country");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Japan");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("USA");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("UK");
            sheet.Cells["B4"].PutValue(3000);

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ocultar detalles del primer campo de fila
            PivotField rowField = pivotTable.RowFields[0];
            rowField.HideDetail(true);
            
            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("HideDetailDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


