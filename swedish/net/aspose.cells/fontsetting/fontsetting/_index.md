---
title: "FontSetting.FontSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSetting-konstruktor."
type: docs
url: /sv/net/aspose.cells/fontsetting/fontsetting/
---
## FontSetting constructor

```csharp
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | Int32 |  |
| length | Int32 |  |
| sheets | WorksheetCollection |  |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingMethodCtorWithInt32Int32WorksheetCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeltext i cellen
            worksheet.Cells["A1"].PutValue("Hello World");
            
            // Skapa teckensnittinställning för de första 5 tecknen (0-4) i alla kalkylblad
            FontSetting fontSetting = new FontSetting(0, 5, workbook.Worksheets);
            
            // Applicera formatering
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Size = 14;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [WorksheetCollection](../../worksheetcollection/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


