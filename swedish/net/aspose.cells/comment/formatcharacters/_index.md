---
title: "Comment.FormatCharacters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment method. Formatera vissa tecken med teckensnittinställningen"
type: docs
url: /sv/net/aspose.cells/comment/formatcharacters/
---
## Comment.FormatCharacters method

Formatera vissa tecken med teckensnittsinställningen.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | Int32 | Startindexet. |
| length | Int32 | Längden. |
| teckensnitt | Teckensnitt | Teckensnittinställningen. |
| flagga | StyleFlag | Flaggan för teckensnittsinställningen. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentRow = 0;
            int commentColumn = 0;
            Comment comment = worksheet.Comments[commentRow, commentColumn];
            comment.Note = "This is a sample comment with formatted text.";

            // Skapa ett teckensnitt för formatering - måste hämtas från arbetsbokens stil
            Aspose.Cells.Font font = workbook.CreateStyle().Font;
            font.IsBold = true;
            font.Color = Color.Red;
            font.Size = 14;
            font.Underline = FontUnderlineType.Single;

            // Skapa stilflagga för att ange vilka teckensnittsegenskaper som ska tillämpas
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontBold = true;
            styleFlag.FontColor = true;
            styleFlag.FontSize = true;
            styleFlag.FontUnderline = true;

            try
            {
                // Formatera tecken från index 5, längd 10
                comment.FormatCharacters(5, 10, font, styleFlag);

                Console.WriteLine("FormatCharacters method executed successfully on the comment.");
                
                // Gör kommentaren synlig för att se effekten
                comment.IsVisible = true;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FormatCharacters method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("CommentFormatCharactersDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../../font/)
* class [StyleFlag](../../styleflag/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


