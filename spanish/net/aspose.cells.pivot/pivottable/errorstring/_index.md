---
title: "PivotTable.ErrorString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Obtiene la cadena mostrada en celdas que contienen errores cuando la propiedad DisplayErrorString es verdadera. El valor predeterminado es una cadena vacía."
type: docs
url: /es/net/aspose.cells.pivot/pivottable/errorstring/
---
## PivotTable.ErrorString property

Obtiene la cadena que se muestra en celdas que contienen errores cuando la propiedad DisplayErrorString es verdadera. El valor predeterminado es una cadena vacía.

```csharp
public string ErrorString { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyErrorStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 1800;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Establecer la propiedad ErrorString
            pivotTable.ErrorString = "Custom Error";
            pivotTable.DisplayErrorString = true;

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Calcular datos y actualizar la tabla dinámica
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableErrorStringDemo.xlsx");

            Console.WriteLine("PivotTable with ErrorString property set successfully.");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


