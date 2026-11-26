---
title: "GlobalizationSettings.GetCommentTitleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre del título del comentario dependiente de la configuración regional según el tipo de título del comentario"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getcommenttitlename/
---
## GlobalizationSettings.GetCommentTitleName method

Obtiene el nombre del título del comentario dependiente de la configuración regional según el tipo de título de comentario.

```csharp
public virtual string GetCommentTitleName(CommentTitleType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | CommentTitleType |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class GlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo : GlobalizationSettings
    {
        public override string GetCommentTitleName(CommentTitleType type)
        {
            switch (type)
            {
                case CommentTitleType.Cell:
                    return "Custom Cell Comment";
                case CommentTitleType.Reply:  // Changed from Threaded to Reply
                    return "Custom Threaded Comment";
                default:
                    return base.GetCommentTitleName(type);
            }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new GlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo(); // Changed to use Settings

            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar comentario de prueba
            int commentIndex = worksheet.Comments.Add("B5");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Test comment content";

            try
            {
                // Obtener el título del comentario para diferentes tipos
                var cellTitle = workbook.Settings.GlobalizationSettings.GetCommentTitleName(CommentTitleType.Cell); // Changed to use Settings
                var threadedTitle = workbook.Settings.GlobalizationSettings.GetCommentTitleName(CommentTitleType.Reply); // Changed type and Settings

                Console.WriteLine($"Cell Comment Title: {cellTitle}");
                Console.WriteLine($"Threaded Comment Title: {threadedTitle}");

                // Establecer el autor del comentario (título) usando nuestras configuraciones de globalización personalizadas
                comment.Author = cellTitle; // Changed from Title to Author
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCommentTitleName method: {ex.Message}");
            }

            workbook.Save("GetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


