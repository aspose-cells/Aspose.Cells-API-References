---
title: "Cell.HasCustomStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Anger om denna cell har anpassade stilinställningar som skiljer sig från standardinställningarna som ärvs från motsvarande rad, kolumn eller arbetsbok"
type: docs
url: /sv/net/aspose.cells/cell/hascustomstyle/
---
## Cell.HasCustomStyle property

Anger om den här cellen har anpassade stilinställningar (annorlunda än standardinställningen som ärvs från motsvarande rad, kolumn eller arbetsbok).

```csharp
public bool HasCustomStyle { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Check HasCustomStyle");

            // Visa initialt HasCustomState-värde (ärver standardstil)
            Console.WriteLine("Initial HasCustomStyle: " + cell.HasCustomStyle);

            // Skapa en anpassad stil och applicera den på cellen
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.IsBold = true;
            cell.SetStyle(customStyle);

            // Verifiera att HasCustomStyle är true efter stiländring
            Console.WriteLine("After applying custom style - HasCustomStyle: " + cell.HasCustomStyle);

            // Spara arbetsboken med den anpassade stilen tillämpad
            workbook.Save("CellCustomStyleDemo.xlsx");

            // Återställ cellens stil till arbetsbokens standardstil
            Style defaultStyle = workbook.DefaultStyle;
            cell.SetStyle(defaultStyle);

            // Verifiera att HasCustomStyle är false efter återgång till standard
            Console.WriteLine("After resetting to default style - HasCustomStyle: " + cell.HasCustomStyle);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


