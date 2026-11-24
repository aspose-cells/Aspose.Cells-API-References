---
title: "PclSaveOptions.AddPrinterFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PclSaveOptions-Methode. Fügt Informationen über die Schriftart hinzu, die bereits vom Hersteller zum Drucker hinzugefügt wurde"
type: docs
url: /de/net/aspose.cells/pclsaveoptions/addprinterfont/
---
## PclSaveOptions.AddPrinterFont method

Fügt Informationen über die Schriftart hinzu, die bereits vom Hersteller zum Drucker hinzugefügt wurde.

```csharp
public void AddPrinterFont(string fontFullName, string fontPclName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFullName | String | Vollständiger Name der Schriftart (z. B. "Times New Roman Bold Italic") in der Quelldatei. |
| fontPclName | String | Name der Schriftart, die im Ausgabedokument Pcl verwendet wird. |

### Hinweise

Laut Pcl-Spezifikation gibt es 52 Schriftarten, die in jedem Drucker eingebaut sein müssen. Hersteller können jedoch weitere Schriftarten zu ihren Geräten hinzufügen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodAddPrinterFontWithStringStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie etwas Text zum Arbeitsblatt hinzu, um die Schriftartverwendung zu demonstrieren.
            worksheet.Cells["A1"].PutValue("This text will use the added printer font");
            
            // Erstelle PCL-Speicheroptionen
            PclSaveOptions pclSaveOptions = new PclSaveOptions();
            
            try
            {
                // Rufen Sie die Methode AddPrinterFont mit bestimmten Schriftartnamen auf.
                pclSaveOptions.AddPrinterFont("Arial", "ArialPCL");
                pclSaveOptions.AddPrinterFont("Times New Roman", "TimesPCL");
                
                Console.WriteLine("AddPrinterFont method executed successfully with parameters (String, String)");
                
                // Speichern Sie die Arbeitsmappe mit PCL-Optionen.
                workbook.Save("PclWithAddedPrinterFonts.pcl", pclSaveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPrinterFont method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


