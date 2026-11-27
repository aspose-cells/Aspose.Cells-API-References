---
title: "Enum NumberCategoryType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.NumberCategoryType enum. Representerar kategori för cellernas talformatering"
type: docs
url: /sv/net/aspose.cells/numbercategorytype/
---
## NumberCategoryType enumeration

Representerar kategoritypen för cellens talformat.

```csharp
public enum NumberCategoryType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| General | `0` | Allmän |
| Text | `1` | Text |
| Number | `2` | Tal |
| Date | `3` | Datum eller Datum och tid |
| Time | `4` | Tid |
| Fraction | `5` | Bråk |
| Scientific | `6` | Vetenskaplig |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NumberCategoryTypeDemo
    {
        public static void NumberCategoryTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("General");
            worksheet.Cells["A2"].PutValue("Text");
            worksheet.Cells["A3"].PutValue(12345);
            worksheet.Cells["A4"].PutValue(DateTime.Now);
            worksheet.Cells["A5"].PutValue(TimeSpan.FromHours(1.5));
            worksheet.Cells["A6"].PutValue(0.75);
            worksheet.Cells["A7"].PutValue(1.23E+3);

            // Ange talformat för cellerna
            worksheet.Cells["A1"].SetStyle(CreateStyle(workbook, NumberCategoryType.General));
            worksheet.Cells["A2"].SetStyle(CreateStyle(workbook, NumberCategoryType.Text));
            worksheet.Cells["A3"].SetStyle(CreateStyle(workbook, NumberCategoryType.Number));
            worksheet.Cells["A4"].SetStyle(CreateStyle(workbook, NumberCategoryType.Date));
            worksheet.Cells["A5"].SetStyle(CreateStyle(workbook, NumberCategoryType.Time));
            worksheet.Cells["A6"].SetStyle(CreateStyle(workbook, NumberCategoryType.Fraction));
            worksheet.Cells["A7"].SetStyle(CreateStyle(workbook, NumberCategoryType.Scientific));

            // Skriv ut talkategori-typerna
            Console.WriteLine("Cell A1 Number Category Type: " + worksheet.Cells["A1"].NumberCategoryType);
            Console.WriteLine("Cell A2 Number Category Type: " + worksheet.Cells["A2"].NumberCategoryType);
            Console.WriteLine("Cell A3 Number Category Type: " + worksheet.Cells["A3"].NumberCategoryType);
            Console.WriteLine("Cell A4 Number Category Type: " + worksheet.Cells["A4"].NumberCategoryType);
            Console.WriteLine("Cell A5 Number Category Type: " + worksheet.Cells["A5"].NumberCategoryType);
            Console.WriteLine("Cell A6 Number Category Type: " + worksheet.Cells["A6"].NumberCategoryType);
            Console.WriteLine("Cell A7 Number Category Type: " + worksheet.Cells["A7"].NumberCategoryType);

            // Spara arbetsboken
            workbook.Save("NumberCategoryTypeExample.xlsx");
        }

        private static Style CreateStyle(Workbook workbook, NumberCategoryType numberCategoryType)
        {
            Style style = workbook.CreateStyle();
            switch (numberCategoryType)
            {
                case NumberCategoryType.General:
                    style.Number = 0;
                    break;
                case NumberCategoryType.Text:
                    style.Number = 49;
                    break;
                case NumberCategoryType.Number:
                    style.Number = 1;
                    break;
                case NumberCategoryType.Date:
                    style.Number = 14;
                    break;
                case NumberCategoryType.Time:
                    style.Number = 21;
                    break;
                case NumberCategoryType.Fraction:
                    style.Number = 9;
                    break;
                case NumberCategoryType.Scientific:
                    style.Number = 11;
                    break;
            }
            return style;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


