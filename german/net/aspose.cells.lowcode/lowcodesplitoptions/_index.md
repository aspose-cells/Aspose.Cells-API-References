---
title: "Klasse LowCodeSplitOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.LowCodeSplitOptions Klasse. Optionen zum Aufteilen von Tabellenkalkulationen"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesplitoptions/
---
## LowCodeSplitOptions class

Optionen zum Aufteilen von Tabellenkalkulationen.

```csharp
public class LowCodeSplitOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LowCodeSplitOptions](lowcodesplitoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [LoadOptions](../../aspose.cells.lowcode/lowcodesplitoptions/loadoptions/) { get; set; } | Ladeoptionen zum Laden der zu teilenden Tabellenkalkulation. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptions/) { get; set; } | Speicheroptionen zum Speichern der geteilten Teile. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/) { get; set; } | Anbieter von Speicheroptionen zum Speichern der geteilten Teile. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeSplitOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Arbeitsblatt mit Beispieldaten füllen
            worksheet.Cells["A1"].PutValue("Sample Data for Splitting");
            
            // Erstellen Sie eine Instanz von LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Konfigurieren Sie LoadOptions (Beispiel: Passwortgeschützte Quelle verarbeiten)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Konfigurieren Sie SaveOptions (Beispiel: Standardausgabeformat festlegen)
            splitOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Implementieren Sie einen benutzerdefinierten SaveOptions-Anbieter für dynamische Ausgabeinstellungen
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Beispielintegration: Arbeitsmappe mit konfigurierten Optionen in Teile aufteilen
            // (Angenommen, es existiert eine Methode wie LowCodeEngine.Split(workbook, splitOptions, \"outputDir\"))
            // LowCodeEngine.Split(workbook, splitOptions, \"OutputDirectory\");
            
            // Speichern Sie die ursprüngliche Arbeitsmappe zur Demonstration
            workbook.Save("LowCodeSplitOptionsDemo.xlsx");
        }

        // Benutzerdefinierte SaveOptionsProvider-Implementierung
        private class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // Beispiel-Logik: Alternierende Einstellungen basierend auf dem Split-Index
                return new LowCodeSaveOptions();
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


