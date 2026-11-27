---
title: "AbstractTextLoadOptions.LoadStyleStrategy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractTextLoadOptions-egenskap. Anger strategin för att tillämpa stil på analyserade värden när en strängvärde konverteras till nummer eller datumtid"
type: docs
url: /sv/net/aspose.cells/abstracttextloadoptions/loadstylestrategy/
---
## AbstractTextLoadOptions.LoadStyleStrategy property

Indikerar strategin för att tillämpa stil på parsade värden när en strängvärde konverteras till nummer eller datum/tid.

```csharp
public TxtLoadStyleStrategy LoadStyleStrategy { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyLoadStyleStrategyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange en anpassad stil för demonstration
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.Name = "Arial";
            customStyle.Font.Size = 12;
            customStyle.Font.Color = System.Drawing.Color.Blue;
            customStyle.Pattern = BackgroundType.Solid;
            customStyle.ForegroundColor = System.Drawing.Color.LightYellow;

            // Tillämpa stilen på en cell
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(customStyle);

            // Skapa CSV-data
            string csvData = "Data1,Data2\nValue1,Value2";
            byte[] byteArray = Encoding.ASCII.GetBytes(csvData);
            MemoryStream stream = new MemoryStream(byteArray);

            // Skapa textinläsningsalternativ med LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn
            };

            // Importera CSV-data med de angivna inläsningsalternativen
            cells.ImportCSV(stream, loadOptions, 0, 0);

            // Spara arbetsboken för att demonstrera resultatet
            workbook.Save("LoadStyleStrategyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [TxtLoadStyleStrategy](../../txtloadstylestrategy/)
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


