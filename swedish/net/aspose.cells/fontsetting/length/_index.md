---
title: "FontSetting.Length"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSetting-egenskap. Hämtar teckenlängden"
type: docs
url: /sv/net/aspose.cells/fontsetting/length/
---
## FontSetting.Length property

Hämtar längden på tecknen.

```csharp
public int Length { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyLengthDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och öppna dess första kalkylblad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite text i cell A1
            worksheet.Cells["A1"].PutValue("Hello World");

            // Skapa teckensnittinställningar för texten i cell A1
            FontSetting fontSetting = worksheet.Cells["A1"].Characters(0, 5);
            
            // Demonstrera användning av Length-egenskapen
            Console.WriteLine("Original Length: " + fontSetting.Length);
            
            // Ändra längden på teckensnittinställningen
            fontSetting = worksheet.Cells["A1"].Characters(0, 11);
            Console.WriteLine("Modified Length: " + fontSetting.Length);
            
            // Tillämpa formatering på teckensnittinställningen
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Spara arbetsboken
            workbook.Save("FontSettingLengthDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


