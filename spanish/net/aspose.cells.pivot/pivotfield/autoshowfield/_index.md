---
title: "PivotField.AutoShowField"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotField. Representa el índice del campo de auto‑mostrar. 1 significa el propio PivotField. Debe ser el índice de los campos de datos."
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/autoshowfield/
---
## PivotField.AutoShowField property

Representa el índice del campo de auto‑mostrar. -1 significa el propio PivotField. Debe ser el índice de los campos de datos.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.RankBy property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoShowField { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, por favor use la propiedad PivotField.Top10AutoShowSettings.RankBy o el método PivotField.Top10AutoShow(). Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoShowFieldDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y completarla con datos de ejemplo
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Agregar datos de muestra para la tabla dinámica
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;
            
            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Configurar AutoShow para el primer campo pivot
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.AutoShowCount = 2;
            pivotField.AutoShowField = 1; // Index of data field (Quantity)
            pivotField.IsAutoShow = true;
            pivotField.IsAscendShow = true; // Equivalent to "Top" in AutoShowType
            
            // Guarda el libro de trabajo
            workbook.Save("PivotField_AutoShowField_Example.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


