---
title: "SaveOptions.SortExternalNames"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SaveOptions-Eigenschaft. Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden sollen"
type: docs
url: /de/net/aspose.cells/saveoptions/sortexternalnames/
---
## SaveOptions.SortExternalNames property

Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.

```csharp
public bool SortExternalNames { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SaveOptionsPropertySortExternalNamesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle ein Beispiel-Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // OoxmlSaveOptions-Instanz erstellen, die von SaveOptions erbt
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // Standardwert der SortExternalNames-Eigenschaft anzeigen
                Console.WriteLine("Default SortExternalNames value: " + saveOptions.SortExternalNames);

                // SortExternalNames auf true setzen
                saveOptions.SortExternalNames = true;
                Console.WriteLine("SortExternalNames set to: " + saveOptions.SortExternalNames);

                // Speichern Sie die Arbeitsmappe mit den angegebenen Speicheroptionen
                workbook.Save("SortExternalNamesDemo.xlsx", saveOptions);

                Console.WriteLine("Workbook saved with SortExternalNames enabled.");
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

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


