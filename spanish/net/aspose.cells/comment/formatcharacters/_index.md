---
title: "Comment.FormatCharacters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Comment. Formatea algunos caracteres con la configuración de fuente"
type: docs
url: /es/net/aspose.cells/comment/formatcharacters/
---
## Comment.FormatCharacters method

Formatea algunos caracteres con la configuración de fuente.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | Int32 | El índice de inicio. |
| longitud | Int32 | La longitud. |
| fuente | Fuente | La configuración de fuente. |
| bandera | StyleFlag | La bandera de la configuración de fuente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CommentMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentRow = 0;
            int commentColumn = 0;
            Comment comment = worksheet.Comments[commentRow, commentColumn];
            comment.Note = "This is a sample comment with formatted text.";

            // Crear una fuente para formatear - es necesario obtenerla del estilo del libro de trabajo
            Aspose.Cells.Font font = workbook.CreateStyle().Font;
            font.IsBold = true;
            font.Color = Color.Red;
            font.Size = 14;
            font.Underline = FontUnderlineType.Single;

            // Crear una bandera de estilo para especificar qué propiedades de fuente aplicar
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontBold = true;
            styleFlag.FontColor = true;
            styleFlag.FontSize = true;
            styleFlag.FontUnderline = true;

            try
            {
                // Formatear caracteres desde el índice 5, longitud 10
                comment.FormatCharacters(5, 10, font, styleFlag);

                Console.WriteLine("FormatCharacters method executed successfully on the comment.");
                
                // Haz visible el comentario para ver el efecto
                comment.IsVisible = true;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FormatCharacters method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("CommentFormatCharactersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../../font/)
* class [StyleFlag](../../styleflag/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


