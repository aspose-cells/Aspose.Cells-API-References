---
title: "Enum VisibilityType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.VisibilityType enum. Representerar tillstånden för bladets synlighet"
type: docs
url: /sv/net/aspose.cells/visibilitytype/
---
## VisibilityType enumeration

Representerar tillstånden för bladets synlighet.

```csharp
public enum VisibilityType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Visible | `0` | Indikerar att bladet är synligt. |
| Hidden | `1` | Indikerar att bladet är dolt, men kan visas av användaren via användargränssnittet. |
| VeryHidden | `2` | Indikerar att bladet är dolt och inte kan visas i användargränssnittet (UI). Detta tillstånd är endast tillgängligt programmässigt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VisibilityTypeDemo
    {
        public static void VisibilityTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("NewSheet");
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange namnet på arbetsbladet
            worksheet.Name = "DemoSheet";

            // Ställ in synligheten för arbetsbladet till Dold
            worksheet.VisibilityType = VisibilityType.Hidden;

            // Spara arbetsboken
            workbook.Save("VisibilityTypeExample.xlsx");

            // Utdata för att indikera att processen är klar
            Console.WriteLine("Workbook saved with the worksheet visibility set to Hidden.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


