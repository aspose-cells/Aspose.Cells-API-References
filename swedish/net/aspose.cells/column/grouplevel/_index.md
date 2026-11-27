---
title: "Column.GroupLevel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Column-egenskap. Hämtar gruppnivån för kolumnen."
type: docs
url: /sv/net/aspose.cells/column/grouplevel/
---
## Column.GroupLevel property

Hämtar gruppnivån för kolumnen.

```csharp
public byte GroupLevel { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gruppera kolumner (isHidden-parameter satt till false)
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // Hämta gruppnivån för den första kolumnen.
            int groupLevel = worksheet.Cells.Columns[0].GroupLevel;
            
            // Skriv ut gruppnivån.
            Console.WriteLine("Group level of first column: " + groupLevel);
            
            // Spara arbetsboken
            workbook.Save("GroupLevelDemo.xlsx");
        }
    }
}
```

### Se även

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


