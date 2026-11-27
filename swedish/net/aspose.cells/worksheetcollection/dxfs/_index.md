---
title: "WorksheetCollection.Dxfs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Hämtar huvudposterna för differentierad formatering"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/dxfs/
---
## WorksheetCollection.Dxfs property

Hämtar huvudposterna för differentialformatering.

```csharp
public DxfCollection Dxfs { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyDxfsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Lägg till villkorsstyrd formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Ange villkor och stil
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightGreen;
            fcc[0].Style = style;
            
            // Demonstrera Dxfs-egenskapen
            Console.WriteLine("Dxfs count before applying formatting: " + workbook.Worksheets.Dxfs.Count);
            
            // Tillämpa formatering som läggs till i Dxfs
            worksheet.ConditionalFormattings[0][0].Priority = 1;
            
            Console.WriteLine("Dxfs count after applying formatting: " + workbook.Worksheets.Dxfs.Count);
        }
    }
}
```

### Se även

* class [DxfCollection](../../dxfcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


