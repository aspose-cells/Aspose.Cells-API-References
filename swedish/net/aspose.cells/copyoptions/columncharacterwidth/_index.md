---
title: "CopyOptions.ColumnCharacterWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CopyOptions‑egenskap. Anger om kolumnbredd ska kopieras i teckenenheter"
type: docs
url: /sv/net/aspose.cells/copyoptions/columncharacterwidth/
---
## CopyOptions.ColumnCharacterWidth property

Anger om kolumnbredd ska kopieras i teckenenheter.

```csharp
public bool ColumnCharacterWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyColumnCharacterWidthDemo
    {
        public static void Run()
        {
            // Skapa en källarbetsbok med exempeldata
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Ställ in kolumnbredd i tecken för demonstration
            srcSheet.Cells.SetColumnWidth(0, 20); // 20 characters wide
            
            // Lägg till lite exempeldata
            srcSheet.Cells["A1"].PutValue("Sample Text");
            srcSheet.Cells["A2"].PutValue("Another Sample");
            
            // Skapa målarbetsbok
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Kopiera med ColumnCharacterWidth satt till true
            destSheet.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = true
            });
            
            // Spara resultatet
            destWorkbook.Save("output_with_column_width.xlsx", SaveFormat.Xlsx);
            
            // För jämförelse, kopiera utan ColumnCharacterWidth
            Workbook destWorkbook2 = new Workbook();
            Worksheet destSheet2 = destWorkbook2.Worksheets[0];
            
            destSheet2.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = false
            });
            
            destWorkbook2.Save("output_without_column_width.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


