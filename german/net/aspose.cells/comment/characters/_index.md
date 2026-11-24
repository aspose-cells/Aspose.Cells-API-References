---
title: "Comment.Characters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Comment-Methode. Gibt ein Characters-Objekt zurück, das einen Zeichenbereich im Kommentartext darstellt"
type: docs
url: /de/net/aspose.cells/comment/characters/
---
## Comment.Characters method

Gibt ein Characters-Objekt zurück, das einen Zeichenbereich im Kommentartext darstellt.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | Int32 | Der Index des Beginns des Zeichens. |
| Länge | Int32 | Die Anzahl der Zeichen. |

### Rückgabewert

Characters-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";
            
            // Abrufen der Schriftarteinstellung für die ersten 4 Zeichen
            FontSetting fontSetting = comment1.Characters(0, 4);
            
            // Ändern Sie die Schriftarteinstellungen
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("CommentFontSettingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


