---
title: "Workbook.GetFonts"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Hämtar alla teckensnitt i stilpoolen."
type: docs
url: /sv/net/aspose.cells/workbook/getfonts/
---
## Workbook.GetFonts method

Hämtar alla teckensnitt i stilpoolen.

```csharp
public Font[] GetFonts()
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetFontsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa celler med olika teckensnitt.
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["A2"].PutValue("Sample Text 2");
            
            // Hämta och ändra teckensnitt.
            Font font1 = worksheet.Cells["A1"].GetStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            
            Font font2 = worksheet.Cells["A2"].GetStyle().Font;
            font2.Name = "Times New Roman";
            font2.Size = 14;
            font2.IsBold = true;

            // Hämta alla teckensnitt som används i arbetsboken.
            Font[] fonts = workbook.GetFonts();
            Console.WriteLine("Total fonts in workbook: " + fonts.Length);
            
            // Visa teckensnittsinformation.
            foreach (Font font in fonts)
            {
                Console.WriteLine($"Font: {font.Name}, Size: {font.Size}, Bold: {font.IsBold}");
            }
            
            // Spara och ladda om för att demonstrera beständighet
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Workbook loadedWorkbook = new Workbook(stream);
                Console.WriteLine("Fonts after save/load: " + loadedWorkbook.GetFonts().Length);
            }
        }
    }
}
```

### Se även

* class [Font](../../font/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


