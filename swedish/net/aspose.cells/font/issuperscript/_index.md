---
title: "Font.IsSuperscript"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font property. Hämtar eller anger ett värde som visar om teckensnittet är upphöjt"
type: docs
url: /sv/net/aspose.cells/font/issuperscript/
---
## Font.IsSuperscript property

Hämtar eller anger ett värde som indikerar om teckensnittet är upphöjt.

```csharp
public bool IsSuperscript { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSuperscriptDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till text i cell A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Normal Text Superscript Text");
            
            // Formatera en del av texten som upphöjd
            FontSetting setting = cell.Characters(12, 11);
            setting.Font.IsSuperscript = true;
            
            // Spara arbetsboken
            workbook.Save("FontIsSuperscriptDemo.xlsx");
            
            // Verifiera den upphöjda inställningen
            Console.WriteLine("IsSuperscript property: " + setting.Font.IsSuperscript);
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


