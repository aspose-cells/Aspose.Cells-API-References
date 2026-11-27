---
title: "Column.Width"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Column-egenskap. Hämtar och anger kolumnbredd i teckenenheter"
type: docs
url: /sv/net/aspose.cells/column/width/
---
## Column.Width property

Hämtar och anger kolumnbredden i tecken.

```csharp
public double Width { get; set; }
```

### Anmärkningar

För kalkylblad mäts kolumnbredden som antalet tecken av den maximala siffrabredden för siffrorna 0~9 när de visas i normalstilens teckensnitt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange bredd för column 3 (index 2)
            worksheet.Cells.Columns[2].Width = 25.5;
            
            // Ange bredd för column 4 (index 3)
            worksheet.Cells.Columns[3].Width = 40.0;
            
            // Hämta och visa breddarna
            Console.WriteLine("Column 3 Width: " + worksheet.Cells.Columns[2].Width);
            Console.WriteLine("Column 4 Width: " + worksheet.Cells.Columns[3].Width);
            
            // Spara arbetsboken
            workbook.Save("ColumnWidthDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


