---
title: "SettableGlobalizationSettings.GetCommentTitleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el nombre del título de comentario dependiente de la configuración regional según el tipo de título de comentario"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/getcommenttitlename/
---
## SettableGlobalizationSettings.GetCommentTitleName method

Obtiene el nombre del título del comentario dependiente de la configuración regional según el tipo de título de comentario.

```csharp
public override string GetCommentTitleName(CommentTitleType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | CommentTitleType | tipo de título de comentario |

### Valor de retorno

nombre del título del comentario dependiente de la configuración regional

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SettableGlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un comentario en la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";
            comment.IsVisible = true;

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Establecer nombres de título de comentario personalizados para diferentes tipos
            settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
            settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
            settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
            settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

            // Aplicar la configuración de globalización al libro de trabajo
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Obtener y mostrar los nombres de los títulos de los comentarios
                Console.WriteLine("Cell title: " + settings.GetCommentTitleName(CommentTitleType.Cell));
                Console.WriteLine("Comment title: " + settings.GetCommentTitleName(CommentTitleType.Comment));
                Console.WriteLine("Note title: " + settings.GetCommentTitleName(CommentTitleType.Note));
                Console.WriteLine("Reply title: " + settings.GetCommentTitleName(CommentTitleType.Reply));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCommentTitleName method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("CommentTitleNamesDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


