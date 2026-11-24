---
title: "Workbook.IsLicensed"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt an, ob die Lizenz gesetzt ist"
type: docs
url: /de/net/aspose.cells/workbook/islicensed/
---
## Workbook.IsLicensed property

Gibt an, ob eine Lizenz festgelegt ist.

```csharp
public bool IsLicensed { get; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsLicensedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Setze einige grundlegende Eigenschaften, um zu demonstrieren, dass das Workbook verwendet wird
            wb.Worksheets[0].Name = "Sheet1";
            wb.Worksheets[0].Cells[0, 0].PutValue("Sample Data");
            
            // Prüfen, ob die Arbeitsmappe lizenziert ist
            Console.WriteLine($"IsLicensed: {wb.IsLicensed}");
            
            // Demonstriere unterschiedliches Verhalten basierend auf dem Lizenzstatus
            if (wb.IsLicensed)
            {
                Console.WriteLine("Running in licensed mode - full features available");
            }
            else
            {
                Console.WriteLine("Running in evaluation mode - watermarks will appear");
            }

            // Speichere in einen Memory-Stream, um die Funktionalität zu demonstrieren
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                Console.WriteLine($"Workbook saved successfully (Size: {ms.Length} bytes)");
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


