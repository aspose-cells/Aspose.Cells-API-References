---
title: "Workbook.Colors"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Devuelve los colores en la paleta para la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/workbook/colors/
---
## Workbook.Colors property

Devuelve los colores de la paleta para la hoja de cálculo.

```csharp
public Color[] Colors { get; }
```

### Observaciones

La paleta tiene 56 entradas, cada una representada por un valor RGB.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyColorsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la paleta de colores predeterminada
            Color[] colors = workbook.Colors;

            // Modificar algunos colores en la paleta
            colors[0] = System.Drawing.Color.Red;      // Modify first color to Red
            colors[1] = System.Drawing.Color.Green;    // Modify second color to Green
            colors[2] = System.Drawing.Color.Blue;    // Modify third color to Blue

            // Cree una hoja de cálculo y agregue algunos datos
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Color Demo");
            
            // Aplicar los colores modificados a las celdas
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = colors[0];
            style1.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = colors[1];
            style2.Pattern = BackgroundType.Solid;
            worksheet.Cells["B2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = colors[2];
            style3.Pattern = BackgroundType.Solid;
            worksheet.Cells["C2"].SetStyle(style3);

            // Guarda el libro de trabajo
            workbook.Save("WorkbookColorsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


