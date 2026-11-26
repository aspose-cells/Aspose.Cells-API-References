---
title: "CellsColor.Argb"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellsColor. Obtiene y establece el color a partir de un valor ARGB de 32 bits"
type: docs
url: /es/net/aspose.cells/cellscolor/argb/
---
## CellsColor.Argb property

Obtiene y establece el color a partir de un valor ARGB de 32 bits.

```csharp
public int Argb { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyArgbDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango y estilo
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A5");
            Style style = workbook.CreateStyle();

            // Crear y configurar CellsColor usando la propiedad Argb
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Argb = Color.FromArgb(128, 0, 0, 255).ToArgb(); // Semi-transparent blue

            // Aplicar el color al estilo
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            
            // Aplicar estilo al rango
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Guarda el libro de trabajo
            workbook.Save("CellsColorArgbDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


