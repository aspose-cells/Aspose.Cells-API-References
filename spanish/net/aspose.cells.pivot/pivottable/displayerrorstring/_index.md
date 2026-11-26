---
title: "PivotTable.DisplayErrorString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si el informe PivotTable muestra una cadena personalizada en celdas que contienen errores"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/displayerrorstring/
---
## PivotTable.DisplayErrorString property

Indica si el informe de PivotTable muestra una cadena personalizada en las celdas que contienen errores.

```csharp
public bool DisplayErrorString { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayErrorStringDemo
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
            cells["B5"].Value = 2500;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Establecer la propiedad DisplayErrorString y demostrar su uso
            pivotTable.DisplayErrorString = true;
            pivotTable.ErrorString = "Custom Error";

            // Calcular datos para mostrar el efecto
            pivotTable.CalculateData();

            Console.WriteLine("DisplayErrorString is set to: " + pivotTable.DisplayErrorString);
            Console.WriteLine("ErrorString is set to: " + pivotTable.ErrorString);

            // Guarda el libro de trabajo
            workbook.Save("PivotTablePropertyDisplayErrorStringDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


