---
title: "SettableGlobalizationSettings.SetCommentTitleName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene il nome del titolo del commento dipendente dalla lingua in base al tipo di titolo del commento"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/setcommenttitlename/
---
## SettableGlobalizationSettings.SetCommentTitleName method

Ottiene il nome del titolo del commento dipendente dalla locale in base al tipo di titolo del commento.

```csharp
public void SetCommentTitleName(CommentTitleType type, string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | CommentTitleType | tipo di titolo del commento |
| name | String | nome del titolo del commento dipendente dalla locale |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            comment.IsVisible = true;

            // Crea impostazioni di globalizzazione
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Imposta nomi personalizzati del titolo del commento per diversi tipi
                settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Applica le impostazioni di globalizzazione al workbook
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetCommentTitleName method executed successfully with parameters (CommentTitleType, String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCommentTitleName method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("MethodSetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


