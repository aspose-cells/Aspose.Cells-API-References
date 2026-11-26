---
title: "PivotField.IsAutoShow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si el campo de tabla dinámica especificado se muestra automáticamente"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/isautoshow/
---
## PivotField.IsAutoShow property

Indica si el campo de tabla dinámica especificado se muestra automáticamente.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.IsAutoShow property  or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAutoShow { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.Top10AutoShowSettings.IsAutoShow o el método PivotField.Top10AutoShow(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoShowDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Agregar tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Añade un campo de datos y configura IsAutoShow
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            
            // Habilita AutoShow y configura los ajustes
            dataField.IsAutoShow = true;
            dataField.AutoShowCount = 2;
            dataField.AutoShowField = 0; // Index of the field to auto show
            dataField.IsAscendShow = true;
            
            // Calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Muestra el valor de la propiedad IsAutoShow
            Console.WriteLine("IsAutoShow property value: " + dataField.IsAutoShow);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldPropertyIsAutoShowDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


