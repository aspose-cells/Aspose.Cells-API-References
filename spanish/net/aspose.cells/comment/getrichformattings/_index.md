---
title: "Comment.GetRichFormattings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Comment. Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto del comentario"
type: docs
url: /es/net/aspose.cells/comment/getrichformattings/
---
## Comment.GetRichFormattings method

Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto del comentario.

```csharp
public FontSetting[] GetRichFormattings()
```

### Valor de retorno

Todos los objetos Characters

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.HtmlNote = "<b>Bold</b>, <i>Italic</i>, <u>Underline</u>";

            // Obtener formatos de texto enriquecido
            FontSetting[] formattings = comment.GetRichFormattings();

            // Mostrar información de formato
            Console.WriteLine("Rich Text Formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"StartIndex: {setting.StartIndex}, Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}, Italic: {setting.Font.IsItalic}, Underline: {setting.Font.Underline}");
            }
        }
    }
}
```

### Ver también

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


