---
title: "Comment.Characters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment‑metod. Returnerar ett Characters‑objekt som representerar ett teckenintervall i kommentartexten"
type: docs
url: /sv/net/aspose.cells/comment/characters/
---
## Comment.Characters method

Returnerar ett Characters-objekt som representerar ett intervall av tecken i kommentartexten.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | Int32 | Indexet för början av tecknet. |
| length | Int32 | Antalet tecken. |

### Returvärde

Characters-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";
            
            // Hämta teckensnittinställning för de första 4 tecknen
            FontSetting fontSetting = comment1.Characters(0, 4);
            
            // Modifiera teckensnittinställningarna
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Spara arbetsboken
            workbook.Save("CommentFontSettingDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


