---
title: "Style.IsModified"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-metod. Kontrollerar om de angivna egenskaperna för stilen har ändrats. Används för stil i ConditionalFormattings för att kontrollera om de angivna egenskaperna för denna stil ska användas när ConditionalFormattings tillämpas på en cell."
type: docs
url: /sv/net/aspose.cells/style/ismodified/
---
## Style.IsModified method

Kontrollerar om de angivna egenskaperna för stilen har ändrats. Används för stil av ConditionalFormattings för att kontrollera om de angivna egenskaperna för denna stil ska användas när ConditionalFormattings tillämpas på en cell.

```csharp
public bool IsModified(StyleModifyFlag modifyFlag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| modifyFlag | StyleModifyFlag | Flaggor för modifierad stil |

### Returvärde

sant om de angivna egenskaperna har modifierats

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodIsModifiedWithStyleModifyFlagDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta stilen för cell A1
            Style style = worksheet.Cells["A1"].GetStyle();
            
            // Modifiera mönstret (bakgrund) för stilen
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            
            // Kontrollera om mönstret har modifierats
            bool isPatternModified = style.IsModified(StyleModifyFlag.Pattern);
            
            // Skriv ut resultatet
            Console.WriteLine("Is pattern modified: " + isPatternModified);
        }
    }
}
```

### Se även

* enum [StyleModifyFlag](../../stylemodifyflag/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


