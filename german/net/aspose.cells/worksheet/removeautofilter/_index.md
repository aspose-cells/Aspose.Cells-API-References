---
title: "Worksheet.RemoveAutoFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Entfernt den Auto-Filter des Arbeitsblatts"
type: docs
url: /de/net/aspose.cells/worksheet/removeautofilter/
---
## Worksheet.RemoveAutoFilter method

Entfernt den Auto-Filter des Arbeitsblatts.

```csharp
public void RemoveAutoFilter()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAutoFilterDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Auto-Filter anwenden
            worksheet.AutoFilter.Range = "A1:A3";
            
            Console.WriteLine("AutoFilter applied: " + worksheet.HasAutofilter);
            
            // Auto-Filter entfernen
            worksheet.RemoveAutoFilter();
            
            Console.WriteLine("AutoFilter after removal: " + worksheet.HasAutofilter);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


