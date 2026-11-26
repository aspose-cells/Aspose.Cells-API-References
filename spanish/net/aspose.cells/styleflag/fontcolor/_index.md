---
title: "StyleFlag.FontColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración del color de fuente"
type: docs
url: /es/net/aspose.cells/styleflag/fontcolor/
---
## StyleFlag.FontColor property

Se aplicará la configuración de color de fuente.

```csharp
public bool FontColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un estilo personalizado
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.BackgroundColor = System.Drawing.Color.LightGray;
            
            // Crear una bandera de estilo y habilitar el color de fuente y el sombreado de celda
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontColor = true;
            styleFlag.CellShading = true;
            
            // Aplicar el estilo a la celda A1 con las banderas especificadas
            worksheet.Cells["A1"].PutValue("Red Text on Gray Background");
            worksheet.Cells["A1"].SetStyle(style, styleFlag);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


