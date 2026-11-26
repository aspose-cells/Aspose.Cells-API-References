---
title: "PivotTable.Indent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PivotTable property. Especifica el incremento de sangría para el eje compacto y puede usarse para establecer el diseño del informe en forma compacta"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/indent/
---
## PivotTable.Indent property

Especifica el incremento de sangría para el eje compacto y puede usarse para establecer el diseño del informe en forma compacta.

```csharp
public int Indent { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIndentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Establecer la propiedad de sangría
            pivotTable.Indent = 3;
            Console.WriteLine("Pivot Table Indent: " + pivotTable.Indent);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableIndentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


