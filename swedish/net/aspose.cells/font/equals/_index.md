---
title: "Font.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font method. Kontrollerar om två teckensnitt är lika"
type: docs
url: /sv/net/aspose.cells/font/equals/
---
## Font.Equals method

Kontrollerar om två teckensnitt är lika.

```csharp
public bool Equals(Font font)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| teckensnitt | Teckensnitt | Jämfört teckensnittobjekt. |

### Returvärde

Sant om lika med det jämförda teckensnittobjektet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontMethodEqualsWithFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa två teckensnittobjekt för jämförelse
            Font font1 = workbook.CreateStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            font1.IsBold = true;
            font1.Color = System.Drawing.Color.Black;

            Font font2 = workbook.CreateStyle().Font;
            font2.Name = "Arial";
            font2.Size = 12;
            font2.IsBold = true;
            font2.Color = System.Drawing.Color.Black;

            try
            {
                // Anropa Equals-metoden för att jämföra teckensnitten
                bool areEqual = font1.Equals(font2);

                // Visa resultatet
                Console.WriteLine($"The fonts are equal: {areEqual}");

                // Modifiera ett teckensnitt för att göra dem olika
                font2.IsItalic = true;
                areEqual = font1.Equals(font2);
                Console.WriteLine($"After modification, the fonts are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("FontEqualsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


