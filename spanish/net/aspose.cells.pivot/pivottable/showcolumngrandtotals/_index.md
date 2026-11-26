---
title: "PivotTable.ShowColumnGrandTotals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si se deben mostrar los totales generales para las columnas de esta tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showcolumngrandtotals/
---
## PivotTable.ShowColumnGrandTotals property

Indica si se deben mostrar los totales generales para las columnas de esta tabla dinámica.

```csharp
public bool ShowColumnGrandTotals { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowColumnGrandTotalsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["A5"].Value = "Apple";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 6;
            cells["B5"].Value = 2;

            // Agregar tabla dinámica
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit as rows
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sum of Quantity

            // Demostrar la propiedad ShowColumnGrandTotals
            pivotTable.ShowColumnGrandTotals = false; // Disable column grand totals
            Console.WriteLine("Column Grand Totals Visible: " + pivotTable.ShowColumnGrandTotals);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableShowColumnGrandTotalsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


