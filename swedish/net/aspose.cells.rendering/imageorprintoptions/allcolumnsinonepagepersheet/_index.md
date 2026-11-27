---
title: "ImageOrPrintOptions.AllColumnsInOnePagePerSheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Om AllColumnsInOnePagePerSheet är true kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. Bredden på papperstorleken i sidinställningarna blir ogiltig och de andra inställningarna för sidinställningarna kommer fortfarande att tillämpas"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/
---
## ImageOrPrintOptions.AllColumnsInOnePagePerSheet property

Om AllColumnsInOnePagePerSheet är sant, kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. Bredden på pappersstorleken i sidinställningarna blir ogiltig, men de övriga inställningarna för sidinställningarna förblir aktiva.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyAllColumnsInOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och lägg till exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i några data i kalkylbladet
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Skapa bildsparalternativ
            ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
            pngOptions.ImageOrPrintOptions.AllColumnsInOnePagePerSheet = true;
            pngOptions.ImageOrPrintOptions.OnePagePerSheet = true;

            // Spara arbetsbok till minnesström som PNG
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, pngOptions);
                Console.WriteLine("Workbook saved as PNG with all columns in one page per sheet.");
            }
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


