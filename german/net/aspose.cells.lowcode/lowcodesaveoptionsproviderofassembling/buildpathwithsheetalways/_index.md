---
title: "LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfAssembling-Eigenschaft. Gibt an, ob das Blatt‑Index oder der Name immer zum Dateipfad hinzugefügt werden soll. Der Standardwert ist false, das bedeutet, wenn nur ein Blatt vorhanden ist, werden der Blatt‑Index bzw. Name und das entsprechende Präfix nicht zum Dateipfad hinzugefügt."
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways property

Ob der Blatt‑Index oder -Name immer zum Dateipfad hinzugefügt wird. Standardwert ist false, d.h., wenn nur ein Blatt vorhanden ist, werden der Blatt‑Index (oder Name) und das entsprechende Präfix nicht zum Dateipfad hinzugefügt.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit einem Arbeitsblatt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Erstelle eine Instanz von LowCodeSaveOptionsProviderOfAssembling
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
            
            // Pfad‑Einstellungen konfigurieren
            provider.PathHeader = "output/";
            provider.PathTail = ".xlsx";
            provider.UseSheetName = true; // Use sheet name instead of index
            provider.SheetPrefix = "_Sheet_";
            provider.SplitPartPrefix = "_Part_";
            
            // Ursprünglichen Eigenschaftswert anzeigen
            Console.WriteLine("Initial BuildPathWithSheetAlways: " + provider.BuildPathWithSheetAlways);
            
            // Dateipfad ohne BuildPathWithSheetAlways demonstrieren
            string defaultPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (default): " + defaultPath);
            
            // Setze BuildPathWithSheetAlways auf true
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine("\nAfter setting BuildPathWithSheetAlways to true: " + provider.BuildPathWithSheetAlways);
            
            // Dateipfad mit BuildPathWithSheetAlways demonstrieren (auch bei einem einzelnen Blatt)
            string updatedPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (updated): " + updatedPath);
            
            // Speichere die Arbeitsmappe (das Aufteilungsverhalten würde die Einstellungen des Anbieters in realen Szenarien verwenden)
            workbook.Save("BuildPathWithSheetAlwaysDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


