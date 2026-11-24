---
title: "Klasse LowCodeMergeOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.LowCodeMergeOptions Klasse. Optionen zum Zusammenführen mehrerer Vorlagendateien zu einer"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodemergeoptions/
---
## LowCodeMergeOptions class

Optionen zum Zusammenführen mehrerer Vorlagendateien zu einer.

```csharp
public class LowCodeMergeOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LowCodeMergeOptions](lowcodemergeoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [LoadOptionsProvider](../../aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/) { get; set; } | Anbieter von Speicheroptionen zum Speichern der geteilten Teile. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodemergeoptions/saveoptions/) { get; set; } | Speicheroptionen zum Speichern der geteilten Teile. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeMergeOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstelle und konfiguriere LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            
            // Setze Speicheroptionen für das Ausgabeformat
            mergeOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Weise einen benutzerdefinierten Ladeoptionen-Provider zu
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();
            
            // Beispielintegration (hypothetische Verwendung mit Merge-Funktionalität)
            // Dies würde typischerweise mit tatsächlichen Dateipfaden aufgerufen werden
            // Workbook.Merge(new string[] { \"template1.xlsx\", \"template2.xlsx\" }, mergeOptions);
            
            // Speichere das Arbeitsbuch (Demonstrationszwecke)
            workbook.Save("LowCodeMergeOptionsDemo.xlsx");
        }
    }

    // Benutzerdefinierter Provider, der die abstrakte Klasse implementiert
    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {
        public override bool MoveNext()
        {
            // Minimale Implementierung, um die abstrakte Anforderung zu erfüllen
            return false;
        }

        public override LowCodeLoadOptions Current
        {
            get { throw new InvalidOperationException(); }
        }

        public LoadOptions GetLoadOptions(string fileName)
        {
            if (fileName.EndsWith(".xlsx", StringComparison.OrdinalIgnoreCase))
            {
                return new LoadOptions(LoadFormat.Xlsx);
            }
            return new LoadOptions();
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


