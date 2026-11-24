---
title: "Comment.FormatCharacters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Methode. Formatiere einige Zeichen mit den Schriftarteinstellungen"
type: docs
url: /de/net/aspose.cells/comment/formatcharacters/
---
## Comment.FormatCharacters method

Formatiere einige Zeichen mit den Schriftarteinstellungen.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | Int32 | Der Startindex. |
| Länge | Int32 | Die Länge. |
| Schriftart | Schriftart | Die Schriftarteinstellung. |
| Flag | StyleFlag | Das Flag der Schriftarteinstellung. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentRow = 0;
            int commentColumn = 0;
            Comment comment = worksheet.Comments[commentRow, commentColumn];
            comment.Note = "This is a sample comment with formatted text.";

            // Erstelle eine Schriftart für die Formatierung – muss aus dem Stil der Arbeitsmappe bezogen werden
            Aspose.Cells.Font font = workbook.CreateStyle().Font;
            font.IsBold = true;
            font.Color = Color.Red;
            font.Size = 14;
            font.Underline = FontUnderlineType.Single;

            // Erstelle ein Stil-Flag, um anzugeben, welche Schriftarteigenschaften angewendet werden sollen
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontBold = true;
            styleFlag.FontColor = true;
            styleFlag.FontSize = true;
            styleFlag.FontUnderline = true;

            try
            {
                // Formatzeichen ab Index 5, Länge 10
                comment.FormatCharacters(5, 10, font, styleFlag);

                Console.WriteLine("FormatCharacters method executed successfully on the comment.");
                
                // Machen Sie den Kommentar sichtbar, um die Wirkung zu sehen
                comment.IsVisible = true;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FormatCharacters method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("CommentFormatCharactersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../../font/)
* class [StyleFlag](../../styleflag/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


