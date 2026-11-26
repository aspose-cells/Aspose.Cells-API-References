---
title: "PivotTable.SubtotalHiddenPageItems"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Indica si los elementos de campo de página ocultos en el informe de PivotTable se incluyen en los subtotales de filas y columnas, totales de bloques y totales generales. El valor predeterminado es False"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/subtotalhiddenpageitems/
---
## PivotTable.SubtotalHiddenPageItems property

Indica si los elementos de campo de página ocultos en el informe de la tabla dinámica se incluyen en los subtotales de fila y columna, totales de bloque y totales generales. El valor predeterminado es False.

```csharp
public bool SubtotalHiddenPageItems { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertySubtotalHiddenPageItemsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Apple";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Orange";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Banana";
            cells["B4"].Value = "North";
            cells["C4"].Value = 1500;
            
            cells["A5"].Value = "Apple";
            cells["B5"].Value = "South";
            cells["C5"].Value = 1200;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Agregar campos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Establecer la propiedad SubtotalHiddenPageItems
            pivotTable.SubtotalHiddenPageItems = true;
            Console.WriteLine("SubtotalHiddenPageItems set to: " + pivotTable.SubtotalHiddenPageItems);

            // Actualizar y calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTable_SubtotalHiddenPageItemsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


