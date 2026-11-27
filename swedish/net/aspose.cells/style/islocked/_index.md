---
title: "Style.IsLocked"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Hämtar eller anger ett värde som indikerar om en cell kan modifieras eller inte"
type: docs
url: /sv/net/aspose.cells/style/islocked/
---
## Style.IsLocked property

Hämtar eller anger ett värde som indikerar om en cell kan ändras eller inte.

```csharp
public bool IsLocked { get; set; }
```

### Anmärkningar

Låsning av celler har ingen effekt om inte kalkylbladet är skyddat.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in egenskapen IsLocked för en cell
            Cell cell = cells["A1"];
            Style style = cell.GetStyle();
            style.IsLocked = true;
            cell.SetStyle(style);

            // Skydda kalkylbladet för att upprätthålla låsning
            worksheet.Protect(ProtectionType.All);

            // Verifiera och skriv ut statusen för IsLocked
            Console.WriteLine("Cell A1 IsLocked: " + cells["A1"].GetStyle().IsLocked);
            Console.WriteLine("Cell B1 IsLocked: " + cells["B1"].GetStyle().IsLocked);

            // Spara arbetsboken
            workbook.Save("IsLockedDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


