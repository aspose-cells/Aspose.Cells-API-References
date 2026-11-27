---
title: "Worksheet.IsRulerVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Anger om linjalen är synlig. Denna egenskap tillämpas endast för förhandsgranskning av sidbrytningar"
type: docs
url: /sv/net/aspose.cells/worksheet/isrulervisible/
---
## Worksheet.IsRulerVisible property

Anger om linjalen är synlig. Denna egenskap tillämpas endast för sidbrytning förhandsgranskning.

```csharp
public bool IsRulerVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRulerVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in kalkylbladet till PageLayoutView där linjalen är synlig
            worksheet.ViewType = ViewType.PageLayoutView;

            // Växla linjalens synlighet
            worksheet.IsRulerVisible = true;

            // Skriv ut det aktuella linjalens synlighetstillstånd
            Console.WriteLine("Worksheet ruler is visible: " + worksheet.IsRulerVisible);

            // Spara arbetsboken
            workbook.Save("WorksheetRulerVisibilityDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


