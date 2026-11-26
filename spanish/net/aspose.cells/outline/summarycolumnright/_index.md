---
title: "Outline.SummaryColumnRight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Outline. Indica si la columna de resumen se posicionará a la derecha de las columnas de detalle en el esquema"
type: docs
url: /es/net/aspose.cells/outline/summarycolumnright/
---
## Outline.SummaryColumnRight property

Indica si la columna de resumen se posicionará a la derecha de las columnas de detalle en el esquema.

```csharp
public bool SummaryColumnRight { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OutlinePropertySummaryColumnRightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo y agrupar filas
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + (i + 1));
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Agrupar filas (crea un esquema)
            worksheet.Cells.GroupRows(0, 9, false);

            // Obtener la configuración del esquema
            Outline outline = worksheet.Outline;

            // Establecer SummaryColumnRight a true (las columnas de resumen aparecerán a la derecha de las columnas de detalle)
            outline.SummaryColumnRight = true;
            Console.WriteLine("SummaryColumnRight is set to: " + outline.SummaryColumnRight);

            // Guarda el libro de trabajo
            workbook.Save("OutlinePropertySummaryColumnRightDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


