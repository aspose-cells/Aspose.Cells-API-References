---
title: "PivotTable.PrintDrill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Especifica un valor booleano que indica si se deben imprimir los indicadores de perforación. Imprimir botones de expandir/contraer cuando se muestra en la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/printdrill/
---
## PivotTable.PrintDrill property

Especifica un valor booleano que indica si los indicadores de desglose deben imprimirse. Imprime los botones de expandir/contraer cuando se muestra en la tabla dinámica.

```csharp
public bool PrintDrill { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPrintDrillDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            var cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bikes";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Cars";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bikes";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Cars";
            cells["B5"].Value = 2500;

            // Agregar una tabla dinámica
            int index = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Demostrar la propiedad PrintDrill
            pivotTable.PrintDrill = false; // Disable printing drill indicators
            pivotTable.ShowDrill = true;   // Show drill indicators on screen
            
            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTablePrintDrillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


