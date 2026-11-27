---
title: "Cells.IsDefaultColumnHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap."
type: docs
url: /sv/net/aspose.cells/cells/isdefaultcolumnhidden/
---
## Cells.IsDefaultColumnHidden property

```csharp
public bool IsDefaultColumnHidden { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultColumnHiddenDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok och hämta det första kalkylbladet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Lägg till lite data så att kalkylbladet inte är tomt
                cells["A1"].PutValue("First");
                cells["B1"].PutValue("Second");
                cells["C1"].PutValue("Third");

                // Läs egenskapen IsDefaultColumnHidden (standard är falskt)
                bool isDefaultColumnHidden = cells.IsDefaultColumnHidden;
                Console.WriteLine("IsDefaultColumnHidden: " + isDefaultColumnHidden);

                // Spara arbetsboken (valfritt, bara för att slutföra demonstrationen)
                workbook.Save("IsDefaultColumnHiddenDemo.xlsx", SaveFormat.Xlsx);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


