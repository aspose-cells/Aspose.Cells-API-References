---
title: "Cell.GetHtmlString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Hämtar HTML-strängen som innehåller data och vissa format i den här cellen"
type: docs
url: /sv/net/aspose.cells/cell/gethtmlstring/
---
## Cell.GetHtmlString method

Hämtar HTML-strängen som innehåller data och vissa format i denna cell.

```csharp
public string GetHtmlString(bool html5)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| html5 | Boolean | Indikerar om värdet är kompatibelt med html5 |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHtmlStringWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange exempelcellvärde med formatering
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            style.Font.Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            // Demonstrera GetHtmlString med boolesk parameter
            string htmlWithoutDiv = cell.GetHtmlString(false);
            string htmlWithDiv = cell.GetHtmlString(true);
            
            Console.WriteLine("HTML without div wrapper:");
            Console.WriteLine(htmlWithoutDiv);
            Console.WriteLine("\nHTML with div wrapper:");
            Console.WriteLine(htmlWithDiv);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


