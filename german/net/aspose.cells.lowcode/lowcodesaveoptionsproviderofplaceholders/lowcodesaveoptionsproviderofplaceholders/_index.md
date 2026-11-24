---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Konstruktor von LowCodeSaveOptionsProviderOfPlaceHolders. Erstellt eine Instanz, um Speicheroptionen gemäß den angegebenen Vorlagen bereitzustellen."
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders constructor

Instanziiert eine Instanz, um Speicheroptionen gemäß den angegebenen Vorlagen bereitzustellen.

```csharp
public LowCodeSaveOptionsProviderOfPlaceHolders(string pathTemplate)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pathTemplate | String | Die Vorlage des resultierenden Dateipfads. |

### Hinweise

Die unterstützten Platzhalter in der Dateipfadvorlage: ${SheetIndex}: wird durch den Blattindex des geteilten Teils ersetzt${SheetName}: wird durch den Blattnamen des geteilten Teils ersetzt${SplitPartIndex}: wird durch den Index des geteilten Teils ersetzt${SheetIndexPrefix}: wird durch [`SheetIndexPrefix`](../sheetindexprefix/) ersetzt${SheetNamePrefix}: wird durch [`SheetNamePrefix`](../sheetnameprefix/) ersetzt${SplitPartPrefix}: wird durch [`SplitPartPrefix`](../splitpartprefix/) ersetzt

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Rufe die #ctor-Methode mit dem String-Parameter auf.
                string pathTemplate = "output_{sheet}_part_{part}.xlsx";
                var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

                // Einige Eigenschaften festlegen
                provider.SheetIndexOffset = 0;
                provider.SplitPartIndexOffset = 0;
                provider.SheetNamePrefix = "Sheet_";
                provider.SplitPartPrefix = "Part_";

                Console.WriteLine("LowCodeSaveOptionsProviderOfPlaceHolders created successfully with path template: " + pathTemplate);
                Console.WriteLine($"SheetNamePrefix: {provider.SheetNamePrefix}, SplitPartPrefix: {provider.SplitPartPrefix}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LowCodeSaveOptionsProviderOfPlaceHolders: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("LowCodeSaveOptionsProviderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


