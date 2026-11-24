---
title: "Klasse AbstractLowCodeLoadOptionsProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.AbstractLowCodeLoadOptionsProvider Klasse. Implementierung zur Bereitstellung mehrerer Ladeoptionen für Prozesse, die mehrere Eingaben wie Vorlagendateien verwenden"
type: docs
url: /de/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/
---
## AbstractLowCodeLoadOptionsProvider class

Implementierung zur Bereitstellung mehrerer Ladeoptionen für Prozesse, die mehrere Eingaben verwenden (wie Vorlagendateien).

```csharp
public abstract class AbstractLowCodeLoadOptionsProvider
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| abstract [Current](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/) { get; } | Ermittelt die Ladeoptionen, aus denen die Daten des aktuell verarbeiteten Teils geladen werden. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/)(LowCodeLoadOptions) | Gibt Ressourcen nach der Verarbeitung des aktuellen Eingabeteils frei. |
| abstract [MoveNext](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/)() | Prüft, ob weitere Eingaben vorhanden sind. |

### Hinweise

Beispielsweise erfordert die Funktion [`SpreadsheetMerger`](../spreadsheetmerger/) mehrere Vorlagendateien zum Zusammenführen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine benutzerdefinierte Implementierung von AbstractLowCodeLoadOptionsProvider
            var provider = new CustomLoadOptionsProvider();

            // Verarbeiten Sie mehrere Eingaben mithilfe des Anbieters
            while (provider.MoveNext())
            {
                // Rufen Sie die aktuellen Ladeoptionen ab
                LowCodeLoadOptions currentOptions = provider.Current;
                Console.WriteLine($"Processing with load options: {currentOptions}");

                // Erstellen Sie eine Arbeitsmappe mit den aktuellen Optionen
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                Worksheet worksheet = workbook.Worksheets[0];

                // Demonstrieren Sie die Verwendung mit einer Arbeitsmappe
                worksheet.Cells["A1"].PutValue("Processed with custom provider");
                
                // Beenden Sie die Verarbeitung dieses Teils
                provider.Finish(currentOptions);
            }
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int currentIndex = 0;
            private readonly LowCodeLoadOptions[] optionsList = new LowCodeLoadOptions[]
            {
                new LowCodeLoadOptions(),
                new LowCodeLoadOptions { InputFile = "protected.xlsx" }, // Password would be handled separately
                new LowCodeLoadOptions() // MemorySetting would be handled separately
            };

            public override LowCodeLoadOptions Current => optionsList[currentIndex];

            public override bool MoveNext()
            {
                if (currentIndex < optionsList.Length - 1)
                {
                    currentIndex++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // Aufräum- oder Abschlusslogik für jeden Teil
                Console.WriteLine($"Finished processing part {currentIndex}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


