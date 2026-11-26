---
title: "Enumeración CommentTitleType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Rendering.CommentTitleType. Representa el tipo de título de comentario al renderizar cuando el comentario está configurado para mostrarse al final de la hoja"
type: docs
url: /es/net/aspose.cells.rendering/commenttitletype/
---
## CommentTitleType enumeration

Representa el tipo de título de comentario durante el renderizado cuando el comentario está configurado para mostrarse al final de la hoja.

```csharp
public enum CommentTitleType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Cell | `0` | Representa la celda del título del comentario. |
| Comment | `1` | Representa el comentario del título del comentario. |
| Note | `2` | Representa la nota del título del comentario. |
| Reply | `3` | Representa la respuesta del título del comentario. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCommentTitleTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Cree configuraciones de globalización personalizadas
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

                // Demuestre todos los valores de la enumeración CommentTitleType
                Console.WriteLine("Available CommentTitleType values:");
                Console.WriteLine($"Cell: {(int)CommentTitleType.Cell}");
                Console.WriteLine($"Comment: {(int)CommentTitleType.Comment}");
                Console.WriteLine($"Note: {(int)CommentTitleType.Note}");
                Console.WriteLine($"Reply: {(int)CommentTitleType.Reply}");

                // Establezca títulos personalizados para cada tipo de comentario
                globalizationSettings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Aplicar la configuración de globalización al libro de trabajo
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Agregue un comentario para demostrar la funcionalidad
                int commentIndex = worksheet.Comments.Add("A1");
                Comment comment = worksheet.Comments[commentIndex];
                comment.Note = "This is a test comment";
                comment.Author = "Test Author";

                // Guarda el libro de trabajo
                workbook.Save("CommentTitleTypeDemo.xlsx");

                Console.WriteLine("CommentTitleType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CommentTitleType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


