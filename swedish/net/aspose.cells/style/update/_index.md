---
title: "Style.Update"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-metod. Tillämpa den namngivna stilen på stilarna för de celler som använder denna namngivna stil. Det fungerar som att klicka på OK‑knappen efter att du har avslutat ändringen av stilen. Gäller endast för namngiven stil."
type: docs
url: /sv/net/aspose.cells/style/update/
---
## Style.Update method

Applicera den namngivna stilen på stilarna för de celler som använder denna namngivna stil. Det fungerar som att klicka på "ok"‑knappen efter att du har avslutat att modifiera stilen. Gäller endast för namngivna stilar.

```csharp
public void Update()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodUpdateDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en stil
            Style style = workbook.CreateStyle();
            style.Number = 3; // Set to Percent format
            
            // Applicera stilen på cell A1
            worksheet.Cells["A1"].SetStyle(style);
            
            // Modifiera stilen
            style.Number = 4; // Change to Currency format
            
            // Uppdatera stiländringarna
            style.Update();
            
            // Verifiera att stilen uppdaterades
            Console.WriteLine("Cell A1 Number Format: " + worksheet.Cells["A1"].GetStyle().Number);
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


