---
title: "PivotField.IsAscendShow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotField. Indica si el campo especificado de PivotTable se muestra automáticamente en orden ascendente"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/isascendshow/
---
## PivotField.IsAscendShow property

Indica si el campo de tabla dinámica especificado se muestra automáticamente en orden ascendente.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.IsTop property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAscendShow { get; set; }
```

### Observaciones

NOTA: Esta propiedad está obsoleta. En su lugar, utilice la propiedad PivotField.Top10AutoShowSettings.IsTop o el método PivotField.Top10AutoShow(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAscendShowDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Agregar tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            
            // Establecer la propiedad IsAscendShow
            rowField.IsAscendShow = true;
            Console.WriteLine("IsAscendShow (Row Field): " + rowField.IsAscendShow);
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];
            
            // Establecer la propiedad IsAscendShow
            dataField.IsAscendShow = false;
            Console.WriteLine("IsAscendShow (Data Field): " + dataField.IsAscendShow);
            
            // Actualizar tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


