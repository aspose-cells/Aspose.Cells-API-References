---
title: "Comment.FormatCharacters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Comment. Formatta alcuni caratteri con l'impostazione del font"
type: docs
url: /it/net/aspose.cells/comment/formatcharacters/
---
## Comment.FormatCharacters method

Formatta alcuni caratteri con l'impostazione del font.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | Int32 | L'indice di partenza. |
| lunghezza | Int32 | La lunghezza. |
| font | Font | L'impostazione del font. |
| flag | StyleFlag | Il flag dell'impostazione del font. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentRow = 0;
            int commentColumn = 0;
            Comment comment = worksheet.Comments[commentRow, commentColumn];
            comment.Note = "This is a sample comment with formatted text.";

            // Crea un font per la formattazione - è necessario ottenerlo dallo stile della cartella di lavoro
            Aspose.Cells.Font font = workbook.CreateStyle().Font;
            font.IsBold = true;
            font.Color = Color.Red;
            font.Size = 14;
            font.Underline = FontUnderlineType.Single;

            // Crea un flag di stile per specificare quali proprietà del font applicare
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontBold = true;
            styleFlag.FontColor = true;
            styleFlag.FontSize = true;
            styleFlag.FontUnderline = true;

            try
            {
                // Formatta i caratteri dall'indice 5, lunghezza 10
                comment.FormatCharacters(5, 10, font, styleFlag);

                Console.WriteLine("FormatCharacters method executed successfully on the comment.");
                
                // Rendi il commento visibile per vedere l'effetto
                comment.IsVisible = true;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FormatCharacters method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("CommentFormatCharactersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../../font/)
* class [StyleFlag](../../styleflag/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


