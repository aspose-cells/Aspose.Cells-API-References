---
title: "LowCodeSplitOptions.SaveOptionsProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSplitOptions-Eigenschaft. Anbieter von Speicheroptionen zum Speichern der geteilten Teile"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/
---
## LowCodeSplitOptions.SaveOptionsProvider property

Anbieter von Speicheroptionen zum Speichern der geteilten Teile.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Hinweise

Wenn diese Eigenschaft angegeben ist, hat [`SaveOptions`](../saveoptions/) keine Wirkung, weil die Ausgabe jedes geteilten Teils vom Anbieter festgelegt wird.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Beispieldaten einfügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // LowCodeSplitOptions-Instanz erstellen
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Aktuellen SaveOptionsProvider-Wert anzeigen (standardmäßig null)
            Console.WriteLine("Current SaveOptionsProvider value: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Benutzerdefinierten SaveOptionsProvider erstellen
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Die Wirkung des Setzens von SaveOptionsProvider demonstrieren
            // In einem realen Szenario würde dies beim Aufteilen von Dateien verwendet werden
            Console.WriteLine("After setting SaveOptionsProvider: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Arbeitsmappe speichern (obwohl das Aufteilen hier nicht demonstriert wird)
            workbook.Save("PropertySaveOptionsProviderDemo.xlsx");
        }
    }

    // Benutzerdefinierte Implementierung von AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Benutzerdefinierte Speicheroptionen für jeden geteilten Teil erstellen
            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            return options;
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Nach dem Speichern jedes Teils Aufräumarbeiten durchführen
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### Siehe auch

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


