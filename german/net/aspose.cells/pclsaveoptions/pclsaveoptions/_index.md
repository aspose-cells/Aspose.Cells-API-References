---
title: "PclSaveOptions.PclSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PclSaveOptions-Konstruktor. Erstellt die Optionen zum Speichern einer Pcl-Datei."
type: docs
url: /de/net/aspose.cells/pclsaveoptions/pclsaveoptions/
---
## PclSaveOptions constructor

Erstellt die Optionen zum Speichern einer Pcl-Datei.

```csharp
public PclSaveOptions()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].PutValue("PCL Save Options Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PclSaveOptions constructor");
            
            try
            {
                // Rufen Sie die #ctor-Methode auf, um eine PclSaveOptions-Instanz zu erstellen.
                PclSaveOptions pclOptions = new PclSaveOptions();
                
                // Konfigurieren Sie bei Bedarf zusätzliche Optionen.
                pclOptions.AddPrinterFont("Arial", "ArialPCL");
                
                Console.WriteLine("PclSaveOptions created successfully");
                
                // Speichern Sie die Arbeitsmappe mit PCL-Optionen.
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

### Siehe auch

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


