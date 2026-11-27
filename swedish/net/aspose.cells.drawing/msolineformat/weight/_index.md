---
title: "MsoLineFormat.Weight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormat-egenskap. Returnerar eller anger linjens tjocklek i enheter av pt"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformat/weight/
---
## MsoLineFormat.Weight property

Returnerar eller anger linjens tjocklek i enheter av pt.

```csharp
public double Weight { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyWeightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Ange kommentartexten
            comment.Note = "Sample comment";
            
            // Få åtkomst till kommentarsformens radformat och ange tjockleken
            comment.CommentShape.LineFormat.Weight = 0.75;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Verifiera att tjockleken har satts korrekt
            Console.WriteLine("Line weight: " + worksheet.Comments[0].CommentShape.LineFormat.Weight);
        }
    }
}
```

### Se även

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


