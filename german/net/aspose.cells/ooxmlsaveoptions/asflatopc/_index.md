---
title: "OoxmlSaveOptions.AsFlatOpc"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OoxmlSaveOptions-Eigenschaft. Gibt an, ob als flache OPC-Datei gespeichert wird, die vom Open XML SDK erzeugt werden kann"
type: docs
url: /de/net/aspose.cells/ooxmlsaveoptions/asflatopc/
---
## OoxmlSaveOptions.AsFlatOpc property

Gibt an, ob als flache OPC-Datei gespeichert wird, die vom Open XML SDK erzeugt werden kann.

```csharp
public bool AsFlatOpc { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Flat OPC Demo");

            try
            {
                // Erstelle eine OoxmlSaveOptions-Instanz
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // Standardwert der AsFlatOpc-Eigenschaft anzeigen
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Setze AsFlatOpc auf true
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Speichere die Arbeitsmappe mit AsFlatOpc aktiviert
                workbook.Save("AsFlatOpc_Enabled.xlsx", saveOptions);

                // Erstelle weitere Speicheroptionen mit AsFlatOpc deaktiviert
                OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
                saveOptions2.AsFlatOpc = false;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions2.AsFlatOpc);

                // Speichere die Arbeitsmappe mit AsFlatOpc deaktiviert
                workbook.Save("AsFlatOpc_Disabled.xlsx", saveOptions2);

                Console.WriteLine("AsFlatOpc property demonstration completed successfully.");
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

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


