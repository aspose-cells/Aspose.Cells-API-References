---
title: "SettableGlobalizationSettings.SetCommentTitleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el nombre del título de comentario dependiente de la configuración regional según el tipo de título de comentario"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/setcommenttitlename/
---
## SettableGlobalizationSettings.SetCommentTitleName method

Obtiene el nombre del título del comentario dependiente de la configuración regional según el tipo de título de comentario.

```csharp
public void SetCommentTitleName(CommentTitleType type, string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | CommentTitleType | tipo de título de comentario |
| name | String | nombre del título del comentario dependiente de la configuración regional |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SettableGlobalizationSettingsMethodSetCommentTitleNameWithCommentTitleTypeStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            comment.IsVisible = true;

            // Crear configuraciones de globalización
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Establecer nombres de título de comentario personalizados para diferentes tipos
                settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Aplicar la configuración de globalización al libro de trabajo
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetCommentTitleName method executed successfully with parameters (CommentTitleType, String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCommentTitleName method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("MethodSetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


