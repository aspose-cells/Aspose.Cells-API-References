---
title: "Enum TextOrientationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.TextOrientationType. Enumera los tipos de orientación de texto"
type: docs
url: /es/net/aspose.cells/textorientationtype/
---
## TextOrientationType enumeration

Enumera los tipos de orientación del texto.

```csharp
public enum TextOrientationType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| ClockWise | `0` | Rota el texto 90 grados en sentido horario. |
| CounterClockWise | `1` | Rota el texto 90 grados en sentido antihorario. |
| NoRotation | `2` | Representa el valor predeterminado. |
| TopToBottom | `3` | Muestra el texto de arriba a abajo de la celda. Texto apilado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextOrientationTypeDemo
    {
        public static void TextOrientationTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");
            worksheet.Cells["A2"].PutValue("This is a test comment.");

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add(0, 0);
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment with text orientation.";

            // Establecer diferentes tipos de orientación de texto para el comentario
            comment.TextOrientationType = TextOrientationType.ClockWise;
            Console.WriteLine("Text Orientation: ClockWise");

            // Guarda el libro de trabajo
            workbook.Save("TextOrientationTypeExample_ClockWise.xlsx");

            // Cambiar la orientación del texto a CounterClockWise
            comment.TextOrientationType = TextOrientationType.CounterClockWise;
            Console.WriteLine("Text Orientation: CounterClockWise");

            // Guarda el libro de trabajo
            workbook.Save("TextOrientationTypeExample_CounterClockWise.xlsx");

            // Cambiar la orientación del texto a NoRotation
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Text Orientation: NoRotation");

            // Guarda el libro de trabajo
            workbook.Save("TextOrientationTypeExample_NoRotation.xlsx");

            // Cambiar la orientación del texto a TopToBottom
            comment.TextOrientationType = TextOrientationType.TopToBottom;
            Console.WriteLine("Text Orientation: TopToBottom");

            // Guarda el libro de trabajo
            workbook.Save("TextOrientationTypeExample_TopToBottom.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


