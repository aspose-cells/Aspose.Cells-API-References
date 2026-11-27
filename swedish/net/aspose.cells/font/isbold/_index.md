---
title: "Font.IsBold"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font property. Hämtar eller anger ett värde som visar om teckensnittet är fetstil"
type: docs
url: /sv/net/aspose.cells/font/isbold/
---
## Font.IsBold property

Hämtar eller anger ett värde som indikerar om teckensnittet är fetstil.

```csharp
public bool IsBold { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsBoldDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cell A1 och ange dess värde
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Bold Text Demo");
            
            // Hämta cellens stil och ange teckensnittet som fetstil
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("FontIsBoldDemo.xlsx");
            
            // Verifiera fetstilsattributet
            Workbook loadedWorkbook = new Workbook("FontIsBoldDemo.xlsx");
            Style loadedStyle = loadedWorkbook.Worksheets[0].Cells["A1"].GetStyle();
            Console.WriteLine("IsBold property: " + loadedStyle.Font.IsBold);
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


