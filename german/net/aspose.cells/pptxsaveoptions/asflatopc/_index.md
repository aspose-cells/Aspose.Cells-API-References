---
title: "PptxSaveOptions.AsFlatOpc"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PptxSaveOptions-Eigenschaft. Gibt an, ob als flache OPC-Datei gespeichert wird, die mit dem Open XML SDK erzeugt werden kann"
type: docs
url: /de/net/aspose.cells/pptxsaveoptions/asflatopc/
---
## PptxSaveOptions.AsFlatOpc property

Gibt an, ob als flache OPC‑Datei gespeichert wird, die mit dem Open XML SDK erzeugt werden kann

```csharp
public bool AsFlatOpc { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PptxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle ein Beispiel-Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Flat OPC Demo";

            try
            {
                // Erstelle eine PptxSaveOptions-Instanz
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // Zeige den Standardwert von AsFlatOpc an
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Setze die Eigenschaft auf true, um ihre Verwendung zu demonstrieren
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Speichere die Arbeitsmappe als PPTX mit aktivierter Option
                workbook.Save("AsFlatOpcDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with AsFlatOpc enabled");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


