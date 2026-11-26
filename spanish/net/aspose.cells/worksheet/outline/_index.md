---
title: "Worksheet.Outline"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene el esquema en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/outline/
---
## Worksheet.Outline property

Obtiene el contorno en esta hoja de cálculo.

```csharp
public Outline Outline { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOutlineDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega datos de muestra y crea grupos de esquema
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[$"A{i + 1}"].Value = $"Item {i + 1}";
                worksheet.Cells[$"B{i + 1}"].Value = (i + 1) * 100;
            }

            // Agrupa filas (crea esquema)
            worksheet.Cells.GroupRows(0, 9, false);

            // Accede a las propiedades del esquema
            Outline outline = worksheet.Outline;
            Console.WriteLine($"Outline summary row is below detail: {outline.SummaryRowBelow}");
            Console.WriteLine($"Outline summary column is to right: {outline.SummaryColumnRight}");

            // Cambia la configuración del esquema
            outline.SummaryRowBelow = true;
            outline.SummaryColumnRight = false;

            // Desagrupa filas para demostrar la funcionalidad del esquema
            worksheet.Cells.UngroupRows(0, 9);

            // Guarda el libro de trabajo
            workbook.Save("WorksheetOutlineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Outline](../../outline/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


