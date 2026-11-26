---
title: "DataBar.MinLength"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataBar. Representa la longitud mínima de la barra de datos"
type: docs
url: /es/net/aspose.cells/databar/minlength/
---
## DataBar.MinLength property

Representa la longitud mínima de la barra de datos.

```csharp
public int MinLength { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMinLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            worksheet.Cells["A3"].PutValue(25);
            worksheet.Cells["A4"].PutValue(35);

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            // Agregar barra de datos
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];
            DataBar dataBar = fc.DataBar;

            // Configurar barra de datos
            dataBar.Color = Color.Green;
            dataBar.MinLength = 10;  // Minimum length set to 10%
            dataBar.MaxLength = 100;

            workbook.Save("DataBarMinLengthDemo.xlsx");
            Console.WriteLine("DataBar with MinLength demo executed successfully.");
        }
    }
}
```

### Ver también

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


