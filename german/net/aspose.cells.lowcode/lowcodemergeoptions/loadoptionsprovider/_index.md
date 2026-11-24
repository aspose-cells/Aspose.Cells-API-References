---
title: "LowCodeMergeOptions.LoadOptionsProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeMergeOptions Eigenschaft. Anbieter von Speicheroptionen zum Speichern der geteilten Teile"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/
---
## LowCodeMergeOptions.LoadOptionsProvider property

Anbieter von Speicheroptionen zum Speichern der geteilten Teile.

```csharp
public AbstractLowCodeLoadOptionsProvider LoadOptionsProvider { get; set; }
```

### Hinweise

Wenn diese Eigenschaft angegeben ist, hat [`LoadOptions`](../../../aspose.cells/loadoptions/) keine Wirkung, weil die Ausgabe jedes geteilten Teils vom Anbieter festgelegt wird.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertyLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();

            // Zeige den aktuellen Wert von LoadOptionsProvider an (sollte zunächst null sein)
            Console.WriteLine("Current LoadOptionsProvider value: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Erstelle eine benutzerdefinierte LoadOptionsProvider-Implementierung
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();

            // Demonstriere das Setzen der Eigenschaft
            Console.WriteLine("After setting LoadOptionsProvider: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Verwende die Merge-Optionen mit dem Anbieter
            // Dies würde typischerweise mit Methoden verwendet werden, die mehrere Dateien verarbeiten
            // Zur Demonstration prüfen wir einfach, ob der Anbieter zum nächsten wechseln kann
            bool hasNext = mergeOptions.LoadOptionsProvider.MoveNext();
            Console.WriteLine("LoadOptionsProvider MoveNext result: " + hasNext);

            // Speichere die Arbeitsmappe
            workbook.Save("PropertyLoadOptionsProviderDemo.xlsx");
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int counter = 0;
            private readonly LowCodeLoadOptions options = new LowCodeLoadOptions();

            public override LowCodeLoadOptions Current => options;

            public override bool MoveNext()
            {
                // Simuliere, dass 3 Dateien zu verarbeiten sind
                if (counter < 3)
                {
                    counter++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // Aufräum- oder Finalisierungslogik würde hier stehen
            }
        }
    }
}
```

### Siehe auch

* class [AbstractLowCodeLoadOptionsProvider](../../abstractlowcodeloadoptionsprovider/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


