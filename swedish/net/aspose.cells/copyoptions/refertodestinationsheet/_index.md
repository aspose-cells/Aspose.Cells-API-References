---
title: "CopyOptions.ReferToDestinationSheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CopyOptions-egenskap. När man kopierar området i samma fil och diagrammet refererar till källbladet betyder False att diagrammets datakälla inte kommer att ändras. True betyder att diagrammets datakälla refererar till målbladet."
type: docs
url: /sv/net/aspose.cells/copyoptions/refertodestinationsheet/
---
## CopyOptions.ReferToDestinationSheet property

När området kopieras i samma fil och diagrammet refererar till källbladet, betyder False att diagrammets datakälla inte ändras. True betyder att diagrammets datakälla refererar till destinationsbladet.

```csharp
public bool ReferToDestinationSheet { get; set; }
```

### Anmärkningar

Standardvärdet är false, det fungerar som MS Excel. Till exempel: om man kopierar ett diagram med datakällan \"sheet1!A1:B10\" från arbetsbladet \"sheet1\" till ett annat arbetsblad \"sheet2\", så kommer datakällan att ändras till \"sheet2!A1:B10\"

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToDestinationSheetDemo
    {
        public static void Run()
        {
            // Skapa källarbetsbok med exempeldata
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B1"].PutValue(100);
            sourceSheet.Cells["A2"].PutValue("=SUM(B1)");

            // Skapa målarbetsbok
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets.Add("DestinationSheet");

            // Ställ in kopieringsalternativ med ReferToDestinationSheet
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ReferToDestinationSheet = true;

            // Kopiera arbetsblad med alternativen
            destSheet.Copy(sourceSheet, copyOptions);

            // Spara resultatet
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


