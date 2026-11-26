---
title: "AutoFitterOptions.MaxRowHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFitterOptions. Obtiene y establece la altura máxima de fila en unidades de Punto al ajustar automáticamente filas"
type: docs
url: /es/net/aspose.cells/autofitteroptions/maxrowheight/
---
## AutoFitterOptions.MaxRowHeight property

Obtiene y establece la altura máxima de fila (en unidades de Point) al ajustar automáticamente las filas.

```csharp
public double MaxRowHeight { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyMaxRowHeightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer datos de muestra y formato
            worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row auto-fitting");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells.SetRowHeight(0, 10); // Set initial small row height

            // Crear AutoFitterOptions con la configuración MaxRowHeight
            AutoFitterOptions options = new AutoFitterOptions
            {
                MaxRowHeight = 50, // Limit maximum row height to 50 pixels
                OnlyAuto = true
            };

            // Ajustar automáticamente la fila con limitación de altura
            worksheet.AutoFitRows(0, 0, options);

            Console.WriteLine("Row height after auto-fit with MaxRowHeight=50: " + worksheet.Cells.GetRowHeight(0));

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


