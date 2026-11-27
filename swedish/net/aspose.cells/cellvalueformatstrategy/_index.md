---
title: "Enum CellValueFormatStrategy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellValueFormatStrategy enum. Anger hur stil ska tillämpas för cellens värde"
type: docs
url: /sv/net/aspose.cells/cellvalueformatstrategy/
---
## CellValueFormatStrategy enumeration

Anger hur stil ska tillämpas på cellens värde.

```csharp
public enum CellValueFormatStrategy
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Inte formaterad. |
| CellStyle | `1` | Endast formaterad med cellens ursprungliga stil. |
| DisplayStyle | `2` | Formaterad med cellens visade stil |
| DisplayString | `3` | Hämtar den visade strängen som visas i MS Excel. Den största skillnaden från DisplayStyle är att detta alternativ också beaktar kolumnbreddens effekt. Om kolumnbredden är för liten för att visa den formaterade strängen helt, kan "#" visas, precis som i MS Excel. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueFormatStrategyDemo
    {
        public static void CellValueFormatStrategyExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B1"].PutValue("Number");
            worksheet.Cells["B2"].PutValue(12345.6789);
            worksheet.Cells["C1"].PutValue("Text");
            worksheet.Cells["C2"].PutValue("Hello World");

            // Använd olika CellValueFormatStrategy för att demonstrera deras effekter
            // Ingen: Inte formaterad
            string valueNone = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.None);
            Console.WriteLine($"None: {valueNone}");

            // CellStyle: Endast formaterad med cellens ursprungliga stil
            string valueCellStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle);
            Console.WriteLine($"CellStyle: {valueCellStyle}");

            // DisplayStyle: Formaterad med cellens visade stil
            string valueDisplayStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayStyle);
            Console.WriteLine($"DisplayStyle: {valueDisplayStyle}");

            // DisplayString: Hämtar den visade strängen som visas i MS Excel
            string valueDisplayString = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayString);
            Console.WriteLine($"DisplayString: {valueDisplayString}");

            // Spara arbetsboken till en fil
            workbook.Save("CellValueFormatStrategyExample.xlsx");
            workbook.Save("CellValueFormatStrategyExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


