---
title: "Enumeración TextStrikeType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.TextStrikeType enumeración. Este tipo especifica el tipo de tachado"
type: docs
url: /es/net/aspose.cells/textstriketype/
---
## TextStrikeType enumeration

Este tipo especifica el tipo de tachado.

```csharp
public enum TextStrikeType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Single | `0` | Un solo tachado aplicado al texto. |
| Double | `1` | Un doble tachado aplicado al texto. Solo funciona para el texto de formas o gráficos. |
| None | `2` | No se aplica tachado al texto. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextStrikeTypeDemo
    {
        public static void TextStrikeTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Obtenga la referencia de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            // Accediendo a la celda "A1" de la hoja de cálculo
            Cell cell = worksheet.Cells["A1"];
            // Añadiendo un valor a la celda "A1"
            cell.PutValue("Hello Aspose!");

            // Accediendo a la fuente de la celda
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Estableciendo el tipo de tachado a Simple
            font.StrikeType = TextStrikeType.Single;

            // Aplique el estilo a la celda
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("TextStrikeTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


