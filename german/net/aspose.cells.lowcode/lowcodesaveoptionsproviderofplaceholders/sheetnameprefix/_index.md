---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfPlaceHolders Eigenschaft. Präfix für den Index des Arbeitsblatts"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix property

Präfix für den Index des Arbeitsblatts.

```csharp
public string SheetNamePrefix { get; set; }
```

### Hinweise

Wenn es nur ein Arbeitsblatt gibt und [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) false ist, dann werden dieses Präfix und der Blattindex (oder Name) nicht zum resultierenden Dateipfad hinzugefügt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetNamePrefixDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit zwei Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "SalesData";
            workbook.Worksheets.Add("FinancialReport");

            // Provider mit Pfadvorlage initialisieren, die einen Blatt-Platzhalter enthält
            string pathTemplate = "output_{sheet}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Anfangswert von SheetNamePrefix anzeigen (standardmäßig leer)
            Console.WriteLine("Initial SheetNamePrefix: " + provider.SheetNamePrefix);

            // Neues Präfix festlegen und sicherstellen, dass die Pfaderstellung Blattinformationen enthält
            provider.SheetNamePrefix = "Q4_";
            provider.BuildPathWithSheetAlways = true;

            // Speicheroptionen mit dem richtigen Format konfigurieren
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx // Set the correct save format
            };

            // Arbeitsmappe mit dem Provider speichern – erzeugt "output_Q4_SalesData.xlsx" und "output_Q4_FinancialReport.xlsx"
            workbook.Save("result_directory", SaveFormat.Xlsx); // Pass correct SaveFormat
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


