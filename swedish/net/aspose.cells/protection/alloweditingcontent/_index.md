---
title: "Protection.AllowEditingContent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection-egenskap. Representerar om användaren får redigera innehållet i låsta celler i ett skyddat kalkylblad"
type: docs
url: /sv/net/aspose.cells/protection/alloweditingcontent/
---
## Protection.AllowEditingContent property

Representerar om användaren får redigera innehållet i låsta celler på ett skyddat kalkylblad.

```csharp
public bool AllowEditingContent { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingContentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skydda arbetsbladet med ett lösenord
            worksheet.Protect(ProtectionType.All, "password", null);
            
            // Kontrollera och visa egenskapen AllowEditingContent
            Console.WriteLine("AllowEditingContent before setting: " + worksheet.Protection.AllowEditingContent);
            
            // Ändra egenskapen AllowEditingContent
            worksheet.Protection.AllowEditingContent = true;
            
            // Kontrollera och visa den uppdaterade egenskapen
            Console.WriteLine("AllowEditingContent after setting: " + worksheet.Protection.AllowEditingContent);
            
            // Spara arbetsboken
            workbook.Save("ProtectionPropertyAllowEditingContentDemo.xlsx");
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


