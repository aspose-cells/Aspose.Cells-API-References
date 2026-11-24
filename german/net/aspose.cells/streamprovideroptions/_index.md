---
title: "Klasse StreamProviderOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.StreamProviderOptions Klasse. Stellt die Stream‑Optionen dar"
type: docs
url: /de/net/aspose.cells/streamprovideroptions/
---
## StreamProviderOptions class

Stellt die Stream-Optionen dar.

```csharp
public class StreamProviderOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [StreamProviderOptions](streamprovideroptions/#constructor)() | Initialisiert eine neue Instanz der `StreamProviderOptions`‑Klasse. |
| [StreamProviderOptions](streamprovideroptions/#constructor_1)(ResourceLoadingType, string) | Initialisiert eine neue Instanz der `StreamProviderOptions`‑Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CustomPath](../../aspose.cells/streamprovideroptions/custompath/) { get; set; } | Der vom Benutzer benutzerdefinierte Pfad (URL), der in der erzeugten html-Datei für die referenzierte Quelle gespeichert wird. Wenn er nicht vom Benutzer definiert wird, wird DefaultPath verwendet. Zum Beispiel wird das Blattdaten vom Benutzer nach d:/sheet001.htm gespeichert, die in der Haupt‑html‑Datei verwendete URL sollte \"d:/sheet001.htm\" oder ein anderer gültiger relativer Pfad sein, der von der Haupt‑html‑Datei aus zugänglich ist. |
| [DefaultPath](../../aspose.cells/streamprovideroptions/defaultpath/) { get; } | Der Standardpfad (URL), der in der erzeugten html-Datei für die referenzierte Quelle gespeichert wird. Zum Beispiel werden die Blattdaten in xxx_files/sheet001.htm gespeichert, die in der Haupt‑html‑Datei verwendete URL sollte etwa \"src=\"xxx_files/sheet001.htm\"\" sein. |
| [ResourceLoadingType](../../aspose.cells/streamprovideroptions/resourceloadingtype/) { get; set; } | Liest und setzt den Typ der zu ladenden Ressource. |
| [Stream](../../aspose.cells/streamprovideroptions/stream/) { get; set; } | Liest/Setzt den Stream |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassStreamProviderOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstelle StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Setze einen memory stream zur Demonstration
            options.Stream = new MemoryStream();
            
            // Verwende den Stream (Beispiel: Arbeitsmappe in den Stream speichern)
            workbook.Save(options.Stream, SaveFormat.Xlsx);
            
            // Demonstriere das Schließen des Streams
            CloseStream(options);
        }

        public static void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


