---
title: "Style.IsBorderApplied"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Anger om kantformatering ska tillämpas"
type: docs
url: /sv/net/aspose.cells/style/isborderapplied/
---
## Style.IsBorderApplied property

Anger om kantformateringen ska tillämpas.

```csharp
public bool IsBorderApplied { get; set; }
```

### Anmärkningar

Endast för namngiven stil.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsBorderAppliedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en anpassad stil
            Style style = workbook.CreateStyle();
            
            // Applicera kantinställningar på stilen
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Black;
            
            // Kontrollera om kanten är tillämpad
            Console.WriteLine("IsBorderApplied before setting: " + style.IsBorderApplied);
            
            // Ställ explicit in IsBorderApplied till true
            style.IsBorderApplied = true;
            
            // Tillämpa stilen på en cell
            worksheet.Cells["A1"].SetStyle(style);
            
            // Verifiera kanttillämpning
            Console.WriteLine("IsBorderApplied after setting: " + style.IsBorderApplied);
            
            // Spara arbetsboken
            workbook.Save("IsBorderAppliedDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


