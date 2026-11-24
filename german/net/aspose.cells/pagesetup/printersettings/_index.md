---
title: "PageSetup.PrinterSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Ruft die Einstellungen des Standarddruckers ab und legt sie fest"
type: docs
url: /de/net/aspose.cells/pagesetup/printersettings/
---
## PageSetup.PrinterSettings property

Liest und setzt die Einstellungen des Standarddruckers.

```csharp
public byte[] PrinterSettings { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrinterSettingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Test Printer Settings");
            
            // Greife auf die Seiteneinrichtung zu
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Setze Druckereinstellungen (als Byte-Array)
            byte[] printerSettings = new byte[10]; // Simplified example
            pageSetup.PrinterSettings = printerSettings;
            
            // Verifiziere, dass die Druckereinstellungen gesetzt sind
            Console.WriteLine("Printer Settings: " + (pageSetup.PrinterSettings != null));
            
            // Speichere die Arbeitsmappe
            workbook.Save("PrinterSettingsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


