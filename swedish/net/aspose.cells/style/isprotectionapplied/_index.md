---
title: "Style.IsProtectionApplied"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Anger om skyddsformatering ska tillämpas"
type: docs
url: /sv/net/aspose.cells/style/isprotectionapplied/
---
## Style.IsProtectionApplied property

Anger om skyddsformateringen ska tillämpas.

```csharp
public bool IsProtectionApplied { get; set; }
```

### Anmärkningar

Endast för namngiven stil.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsProtectionAppliedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett stilobjekt
            Style style = workbook.CreateStyle();
            
            // Ställ in skyddsegenskaper
            style.IsLocked = true;
            style.IsFormulaHidden = true;
            style.IsProtectionApplied = true;
            
            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Verifiera skyddsinställningarna
            Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
            Console.WriteLine("IsLocked: " + style.IsLocked);
            Console.WriteLine("IsFormulaHidden: " + style.IsFormulaHidden);
            
            // Ändra skyddsinställningar
            style.IsProtectionApplied = false;
            Console.WriteLine("\nAfter changing IsProtectionApplied to false:");
            Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


