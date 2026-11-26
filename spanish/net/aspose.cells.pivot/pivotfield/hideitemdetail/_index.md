---
title: "PivotField.HideItemDetail"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Establece si el PivotItem específico en un campo dinámico tiene detalle oculto"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/hideitemdetail/
---
## PivotField.HideItemDetail method

Establece si el PivotItem específico en un campo dinámico tiene detalle oculto.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItemDetail(int index, bool isHiddenDetail)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | el índice del pivotItem en el pivotField. |
| isHiddenDetail | Booleano | si el PivotItem específico está oculto |

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotField.PivotItems[int].IsDetailHidden. Este método será eliminado 12 meses después, a partir de agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemDetailWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("SampleData.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("East");
            worksheet.Cells["A5"].PutValue("West");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Agregar tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B5", "H5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campos a áreas
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Obtener el campo de pivote
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Ocultar detalle del elemento en el índice 2 (East) con isHidden=false
            pivotField.HideItemDetail(2, false);
            
            // Actualizar y calcular los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTable_HideItemDetail_Output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


