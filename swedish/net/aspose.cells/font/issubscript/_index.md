---
title: "Font.IsSubscript"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Hämtar eller anger ett värde som indikerar om teckensnittet är nedsänkt"
type: docs
url: /sv/net/aspose.cells/font/issubscript/
---
## Font.IsSubscript property

Hämtar eller anger ett värde som indikerar om teckensnittet är nedsänkt.

```csharp
public bool IsSubscript { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSubscriptDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil med nedsänkt text
            Style subscriptStyle = workbook.CreateStyle();
            subscriptStyle.Font.IsSubscript = true;

            // Skapa en stil med upphöjd text för jämförelse
            Style superscriptStyle = workbook.CreateStyle();
            superscriptStyle.Font.IsSuperscript = true;

            // Tillämpa stilar på celler
            worksheet.Cells["A1"].PutValue("Subscript Text");
            worksheet.Cells["A1"].SetStyle(subscriptStyle);

            worksheet.Cells["A2"].PutValue("Superscript Text");
            worksheet.Cells["A2"].SetStyle(superscriptStyle);

            // Verifiera och visa stilarna
            Console.WriteLine("A1 IsSubscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A1 IsSuperscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSuperscript);
            Console.WriteLine("A2 IsSubscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A2 IsSuperscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSuperscript);

            // Spara arbetsboken
            workbook.Save("FontPropertyIsSubscriptDemo.ods");
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


