---
title: "PageSetup.PrinterSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskapen. Hämtar och anger inställningarna för standardskrivaren"
type: docs
url: /sv/net/aspose.cells/pagesetup/printersettings/
---
## PageSetup.PrinterSettings property

Hämtar och anger inställningarna för standardskrivaren.

```csharp
public byte[] PrinterSettings { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrinterSettingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Test Printer Settings");
            
            // Kom åt sidinställning
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Ställ in skrivareinställningar (som byte array)
            byte[] printerSettings = new byte[10]; // Simplified example
            pageSetup.PrinterSettings = printerSettings;
            
            // Verifiera att skrivareinställningarna är satta
            Console.WriteLine("Printer Settings: " + (pageSetup.PrinterSettings != null));
            
            // Spara arbetsboken
            workbook.Save("PrinterSettingsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


