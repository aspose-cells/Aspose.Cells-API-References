---
title: "AutoFitterOptions.IgnoreHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFitterOptions. Ignora las filas/columnas ocultas"
type: docs
url: /es/net/aspose.cells/autofitteroptions/ignorehidden/
---
## AutoFitterOptions.IgnoreHidden property

Ignora las filas/columnas ocultas.

```csharp
public bool IgnoreHidden { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyIgnoreHiddenDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer datos de muestra y formatear filas
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["A2"].PutValue("Another test string");
            
            // Ocultar fila 1
            worksheet.Cells.Rows[1].IsHidden = true;

            // Crear AutoFitterOptions con IgnoreHidden establecido en true
            AutoFitterOptions options = new AutoFitterOptions
            {
                IgnoreHidden = true,
                AutoFitMergedCells = false,
                OnlyAuto = false
            };

            // Ajustar filas automáticamente mientras se ignoran las filas ocultas
            worksheet.AutoFitRows(options);

            // Mostrar la altura de las filas
            Console.WriteLine("Row 0 height: " + worksheet.Cells.GetRowHeight(0));
            Console.WriteLine("Row 1 height: " + worksheet.Cells.GetRowHeight(1));
        }
    }
}
```

### Ver también

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


