---
title: "Worksheet.HasAutofilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt an, ob dieses Arbeitsblatt einen Auto-Filter hat"
type: docs
url: /de/net/aspose.cells/worksheet/hasautofilter/
---
## Worksheet.HasAutofilter property

Gibt an, ob dieses Arbeitsblatt einen AutoFilter hat.

```csharp
public bool HasAutofilter { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHasAutofilterDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Auto-Filter festlegen
            worksheet.AutoFilter.Range = "A1:B3";
            
            // Prüfen, ob das Arbeitsblatt einen Auto-Filter hat
            Console.WriteLine("Worksheet has autofilter: " + worksheet.HasAutofilter);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


