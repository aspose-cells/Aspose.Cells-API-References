---
title: "Style.CultureCustom"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskapen. Hämtar och anger det kulturberoende mönstersträngen för talformat. Om inget talformat har angetts för detta objekt returneras null. Om talformatet är inbyggt returneras mönstersträngen som motsvarar det inbyggda talet."
type: docs
url: /sv/net/aspose.cells/style/culturecustom/
---
## Style.CultureCustom property

Hämtar och anger det kulturspecifika mönstersträngen för talformat. Om inget talformat har angetts för detta objekt returneras null. Om talformatet är inbyggt returneras mönstersträngen som motsvarar det inbyggda talet.

```csharp
public string CultureCustom { get; set; }
```

### Anmärkningar

För inbyggt talformat är både mönsterinnehållet (t.ex. ett inbyggt datumformat är "m/d/y" för vissa språk, men för andra språk blir det "d/m/y") och formatavgränsaren (t.ex. vissa språk använder ett annat tecken än 'y' för att representera årsdelen i datumformat) kulturbundna; för användarspecificerat anpassat format ändras endast formatavgränsarna enligt kulturen, medan övriga delar av formatmönstret inte modifieras.

### Exempel

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCultureCustomDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och ställ in ungersk kultur
            Workbook wb = new Workbook();
            wb.Settings.CultureInfo = new CultureInfo("hu-HU");

            // Hämta den första cellen och dess stil
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();

            // Ange anpassat format och demonstrera CultureCustom-konvertering
            string customFormat = "yyyy-MM-dd hh:mm:ss ddd dddd MMM MMMM MMMMM";
            string cultureCustomFormat = "éééé-hh-nn óó:pp:mm nnn nnnn hhh hhhh hhhhh";
            
            style.Custom = customFormat;
            Console.WriteLine("CultureCustom from Custom: " + style.CultureCustom);
            
            style.CultureCustom = cultureCustomFormat;
            Console.WriteLine("Custom from CultureCustom: " + style.Custom);

            // Applicera stilen och demonstrera kulturmedveten formatering
            cell.SetStyle(style);
            cell.PutValue(47512); // January 29, 2030
            Console.WriteLine("Formatted value: " + cell.StringValue);

            // Demonstrera formel med kulturformatering
            cell.Formula = "=TEXT(47512,\"" + cultureCustomFormat + "\")";
            wb.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.StringValue);
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


