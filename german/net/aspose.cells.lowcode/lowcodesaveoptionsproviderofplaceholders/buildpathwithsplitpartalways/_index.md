---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfPlaceHolders Eigenschaft. Ob der Index des Split-Teils immer zum Dateipfad hinzugefügt wird. Standardwert ist false, das heißt, wenn es nur einen Split-Teil gibt, werden der Split-Teil-Index und das entsprechende PräfixSplitPartPrefix nicht zum Dateipfad hinzugefügt."
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways property

Ob der Index des Split-Teils immer zum Dateipfad hinzugefügt wird. Standardwert ist false, das heißt, wenn es nur einen Split-Teil gibt, werden der Split-Teil-Index und das entsprechende Präfix([`SplitPartPrefix`](../splitpartprefix/)) nicht zum Dateipfad hinzugefügt.

```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSplitPartAlwaysDemo
    {
        public static void Run()
        {
            // Arbeitsmappe mit Daten erstellen, die nicht in mehrere Teile aufgeteilt werden.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Single Part Demonstration";

            // Provider mit Pfadvorlage und Aufteilungsbedingung erstellen, die zu einem Teil führt.
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Result_{split}.xlsx")
            {
                SaveOptionsTemplate = new LowCodeSaveOptions()
            };

            // Eigenschaft im falschen Zustand demonstrieren (Standard).
            Console.WriteLine($"Initial BuildPathWithSplitPartAlways: {provider.BuildPathWithSplitPartAlways}");
            provider.BuildPathWithSplitPartAlways = false;
            
            // Dies würde Result.xlsx erzeugen, wenn nur ein Teil vorhanden ist.
            Console.WriteLine("Saving with BuildPathWithSplitPartAlways=false");
            ExecuteDummySave(workbook, "Result.xlsx");

            // Eigenschaft umschalten und den wahren Zustand demonstrieren.
            provider.BuildPathWithSplitPartAlways = true;
            Console.WriteLine("\nSaving with BuildPathWithSplitPartAlways=true");
            
            // Dies würde Result_0.xlsx erzeugen, selbst bei einem einzelnen Teil.
            ExecuteDummySave(workbook, "Result_0.xlsx");
        }

        private static void ExecuteDummySave(Workbook workbook, string filename)
        {
            // Im realen Einsatz durch einen provider-basierten Speicheroperation ersetzen.
            Console.WriteLine($"Simulated save operation -> Filename: {filename}");
            workbook.Save(filename, SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


