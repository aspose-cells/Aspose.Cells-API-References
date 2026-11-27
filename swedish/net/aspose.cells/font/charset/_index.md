---
title: "Font.Charset"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Representerar teckenuppsättningen"
type: docs
url: /sv/net/aspose.cells/font/charset/
---
## Font.Charset property

Representerar teckenuppsättningen.

```csharp
public int Charset { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCharsetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil med specifika teckensnittsegenskaper inklusive teckenuppsättning
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Charset = 1; // ANSI_CHARSET

            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Text with ANSI charset");

            // Skapa en annan stil med annan teckenuppsättning
            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 12;
            style2.Font.Charset = 2; // DEFAULT_CHARSET

            // Applicera den andra stilen på en annan cell
            Cell cell2 = worksheet.Cells["A2"];
            cell2.SetStyle(style2);
            cell2.PutValue("Text with DEFAULT charset");

            // Spara arbetsboken
            workbook.Save("FontCharsetDemo.xlsx");

            // Verifiera teckenuppsättningsegenskaperna
            Console.WriteLine("Cell A1 Font Charset: " + cell.GetStyle().Font.Charset);
            Console.WriteLine("Cell A2 Font Charset: " + cell2.GetStyle().Font.Charset);
        }
    }
}
```

### Se även

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


