---
title: "Klasse LowCodeLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.LowCodeLoadOptions Klasse. Optionen zum Laden der Vorlagendatei"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodeloadoptions/
---
## LowCodeLoadOptions class

Optionen zum Laden von Vorlagendateien.

```csharp
public class LowCodeLoadOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LowCodeLoadOptions](lowcodeloadoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [InputFile](../../aspose.cells.lowcode/lowcodeloadoptions/inputfile/) { get; set; } | Liest und setzt die Datei (mit Pfad, falls nötig) der Vorlage. |
| [InputStream](../../aspose.cells.lowcode/lowcodeloadoptions/inputstream/) { get; set; } | Liest und setzt den Stream der Vorlage. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            // Erstelle einen Beispiel‑Stream (im Speicher für Demo‑Zwecke)
            using (MemoryStream stream = new MemoryStream())
            {
                // Erstelle eine neue Arbeitsmappe und speichere sie für die Demo in einen Stream
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Save(stream, SaveFormat.Xlsx);

                // Stream‑Position zurücksetzen
                stream.Position = 0;

                // LowCodeLoadOptions erstellen und verwenden
                var loadOptions = new LowCodeLoadOptions()
                {
                    InputStream = stream
                };

                // Beispielhafte Verwendung – würde typischerweise an eine Verarbeitungsmethode übergeben werden
                Console.WriteLine($"Loading with LowCode options from stream of length: {loadOptions.InputStream.Length}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


