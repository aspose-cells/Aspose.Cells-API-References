---
title: "ReferredArea.StartRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReferredArea. La fila inicial del área"
type: docs
url: /es/net/aspose.cells/referredarea/startrow/
---
## ReferredArea.StartRow property

La fila inicial del área.

```csharp
public int StartRow { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyStartRowDemo
    {
        public static void Run()
        {
            // Crea un libro de trabajo y una hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar algunos datos de muestra
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Crear un rango con nombre que haga referencia a A2:A4
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$2:$A$4";

            // Obtener el área referida con el parámetro recalculate
            ReferredArea area = name.GetReferredAreas(false)[0];

            // Demostrar la propiedad StartRow
            Console.WriteLine("Start Row: " + area.StartRow); // Should output 1 (0-based)
            Console.WriteLine("End Row: " + area.EndRow);     // Should output 3 (0-based)
            Console.WriteLine("Row Count: " + (area.EndRow - area.StartRow + 1)); // Should output 3

            // Iterar a través del área referida usando StartRow y EndRow
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                Cell cell = worksheet.Cells[row, 0]; // Column 0 is A
                Console.WriteLine("Value at row " + row + ": " + cell.Value);
            }
        }
    }
}
```

### Ver también

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


