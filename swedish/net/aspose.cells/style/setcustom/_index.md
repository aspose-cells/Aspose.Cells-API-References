---
title: "Style.SetCustom"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-metod. Anger den anpassade talformatsträngen för en cell"
type: docs
url: /sv/net/aspose.cells/style/setcustom/
---
## Style.SetCustom method

Ställer in den anpassade talformatsträngen för en cell.

```csharp
public void SetCustom(string custom, bool builtinPreference)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| custom | String | Custom number format string, bör vara ett InvariantCulture-mönster. |
| builtinPreference | Boolean | Om den angivna Custom number format string matchar ett av de inbyggda talformaten som motsvarar aktuella regionala inställningar, bör talformatet sättas som inbyggt istället för Custom. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodSetCustomWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Style style = wb.CreateStyle();
            
            string customFormat1 = "_(\"$\"* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat1, true);
            Console.WriteLine("Custom format 1 applied. Style number: " + style.Number);

            string customFormat2 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat2, true);
            Console.WriteLine("Custom format 2 applied. Style number: " + style.Number);

            string customFormat3 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* -??_);_(@_)";
            style.SetCustom(customFormat3, true);
            Console.WriteLine("Custom format 3 applied. Style number: " + style.Number);
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


