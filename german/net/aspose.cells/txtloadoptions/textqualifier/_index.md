---
title: "TxtLoadOptions.TextQualifier"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions-Eigenschaft. Gibt den Textqualifizierer für Zellwerte an. Standardqualifizierer ist"
type: docs
url: /de/net/aspose.cells/txtloadoptions/textqualifier/
---
## TxtLoadOptions.TextQualifier property

Gibt den Textqualifizierer für Zellenwerte an. Standardqualifizierer ist '"'.

```csharp
public char TextQualifier { get; set; }
```

### Hinweise

Beim Festlegen dieser Eigenschaft wird [`HasTextQualifier`](../hastextqualifier/) automatisch auf true gesetzt.

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTextQualifierDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von TxtLoadOptions für CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Erstelle Beispieldaten im CSV-Format mit Textqualifizierern
            string csvData = "Name,Age,City\n\"John Doe\",30,\"New York\"\n\"Jane Smith\",25,\"San Francisco\"";
            
            // Speichere Beispieldaten in einer temporären Datei
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvData);

            // Lade die CSV-Datei mit den angegebenen Optionen
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Speichere die Arbeitsmappe in einer Excel‑Datei
            workbook.Save("TextQualifierDemo.xlsx");

            // Bereinige die temporäre Datei
            System.IO.File.Delete(tempFile);
        }
    }
}
```

### Siehe auch

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


