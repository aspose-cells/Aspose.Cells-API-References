---
title: "PasteOptions.Transpose"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PasteOptions. True para transponer filas y columnas cuando se pega el rango. El valor predeterminado es False"
type: docs
url: /es/net/aspose.cells/pasteoptions/transpose/
---
## PasteOptions.Transpose property

True para transponer filas y columnas cuando se pega el rango. El valor predeterminado es False.

```csharp
public bool Transpose { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyTransposeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear estilo de origen y aplicarlo al rango horizontal
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range sourceRange = cells.CreateRange(0, 0, 1, 4);
            sourceRange.SetStyle(style);

            // Crear opciones de pegado con transposición
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.Formats;
            pasteOptions.Transpose = true;

            // Copiar con transposición a rango vertical
            Aspose.Cells.Range targetRange = cells.CreateRange(2, 0, 4, 1);
            targetRange.Copy(sourceRange, pasteOptions);

            // Guarda el libro de trabajo
            workbook.Save("TransposeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


