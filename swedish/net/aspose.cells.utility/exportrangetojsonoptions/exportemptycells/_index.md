---
title: "ExportRangeToJsonOptions.ExportEmptyCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportRangeToJsonOptions-egenskap. Anger om tomma celler exporteras som null"
type: docs
url: /sv/net/aspose.cells.utility/exportrangetojsonoptions/exportemptycells/
---
## ExportRangeToJsonOptions.ExportEmptyCells property

Anger om tomma celler ska exporteras som null.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ExportRangeToJsonOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data i cellerna
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            // Lämna B2 tom avsiktligt
            
            // Skapa exportalternativ och aktivera export av tomma celler
            ExportRangeToJsonOptions exportOptions = new ExportRangeToJsonOptions();
            exportOptions.ExportEmptyCells = true;
            
            // Exportera området till JSON
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);
            
            Console.WriteLine(jsonData);
        }
    }
}
```

### Se även

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


