---
title: "StyleFlag.HideFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag property. Inställning för att dölja formel kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/hideformula/
---
## StyleFlag.HideFormula property

Inställning för att dölja formel kommer att tillämpas.

```csharp
public bool HideFormula { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyHideFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell a1 = worksheet.Cells["A1"];
            // Lägg till en formel i cell A1
            a1.Formula = "=1+2";
            a1.Value = 3; // Display value

            // Skapa stilflagga med HideFormula satt till true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HideFormula = true;

            // Skapa en stil och sätt IsFormulaHidden till true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;

            // Applicera stilen på cell A1 med stilflaggan
            a1.SetStyle(style, styleFlag);

            // Skydda kalkylbladet för att se effekten av HideFormula
            worksheet.Protection.AllowEditingObject = true;
            worksheet.Protection.AllowEditingContent = false;
            worksheet.Protection.Password = "password";

            // Spara arbetsboken
            workbook.Save("PropertyHideFormulaDemo.xlsx");

            // Verifiera att formeln är dold
            Console.WriteLine("Formula in A1: " + a1.Formula);
            Console.WriteLine("Is formula hidden? " + a1.GetStyle().IsFormulaHidden);
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


