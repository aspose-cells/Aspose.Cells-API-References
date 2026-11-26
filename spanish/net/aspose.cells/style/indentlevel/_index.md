---
title: "Style.IndentLevel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Representa el nivel de sangría para la celda o rango. Solo puede ser un entero de 0 a 250"
type: docs
url: /es/net/aspose.cells/style/indentlevel/
---
## Style.IndentLevel property

Representa el nivel de sangría para la celda o el rango. Solo puede ser un entero de 0 a 250.

```csharp
public int IndentLevel { get; set; }
```

### Observaciones

Si el tipo de alineación horizontal del texto se establece en un valor distinto de izquierda o derecha, el nivel de sangría se restablecerá a cero.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIndentLevelDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establezca diferentes niveles de sangría para las celdas
            for (int i = 0; i < 16; i++)
            {
                Cell cell = cells[i, 0];
                Style style = cell.GetStyle();
                style.IndentLevel = i;
                style.HorizontalAlignment = TextAlignmentType.Left;
                cell.SetStyle(style);
                cell.PutValue($"Indent Level {i}");
            }

            // Guarda el libro de trabajo
            workbook.Save("IndentLevelDemo.xlsx");
            Console.WriteLine("Workbook saved with different indent levels.");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


