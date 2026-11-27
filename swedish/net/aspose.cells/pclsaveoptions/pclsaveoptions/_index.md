---
title: "PclSaveOptions.PclSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PclSaveOptions-konstruktorn. Skapar alternativen för att spara pcl-filen."
type: docs
url: /sv/net/aspose.cells/pclsaveoptions/pclsaveoptions/
---
## PclSaveOptions constructor

Skapar alternativen för att spara pcl-fil.

```csharp
public PclSaveOptions()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("PCL Save Options Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PclSaveOptions constructor");
            
            try
            {
                // Anropa #ctor-metoden för att skapa en PclSaveOptions-instans.
                PclSaveOptions pclOptions = new PclSaveOptions();
                
                // Konfigurera ytterligare alternativ om det behövs.
                pclOptions.AddPrinterFont("Arial", "ArialPCL");
                
                Console.WriteLine("PclSaveOptions created successfully");
                
                // Spara arbetsboken med PCL-alternativ.
                workbook.Save("PclSaveOptionsDemo.pcl", pclOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating PclSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


