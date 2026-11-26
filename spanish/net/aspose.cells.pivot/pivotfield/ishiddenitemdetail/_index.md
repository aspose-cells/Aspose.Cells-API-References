---
title: "PivotField.IsHiddenItemDetail"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Indica si se debe ocultar el detalle del PivotItem específico"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/ishiddenitemdetail/
---
## PivotField.IsHiddenItemDetail method

Indica si se debe ocultar el detalle del PivotItem específico..

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHiddenItemDetail(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice del pivotItem en el pivotField. |

### Valor de retorno

si el detalle del PivotItem específico está oculto

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotField.PivotItems[int].IsDetailHidden. Este método será eliminado 12 meses después, a partir de agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemDetailWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Country";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Japan";
            cells["A3"].Value = "Japan";
            cells["A4"].Value = "USA";
            cells["A5"].Value = "USA";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;
            cells["B5"].Value = 4000;

            // Agregar tabla dinámica
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Obtener campo pivot
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Ocultar detalle del elemento para el índice 1 (USA)
            pivotField.HideItemDetail(1, true);
            
            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Verificar si el detalle del elemento está oculto
            Console.WriteLine("Is item at index 1 hidden? " + pivotField.IsHiddenItemDetail(1));
            
            // Guardar el libro de trabajo
            workbook.Save("PivotFieldIsHiddenItemDetailDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


