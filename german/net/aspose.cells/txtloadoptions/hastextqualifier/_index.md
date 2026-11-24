---
title: "TxtLoadOptions.HasTextQualifier"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions-Eigenschaft. Gibt an, ob ein Textqualifizierer für den Zellwert vorhanden ist. Standard ist true"
type: docs
url: /de/net/aspose.cells/txtloadoptions/hastextqualifier/
---
## TxtLoadOptions.HasTextQualifier property

Ob ein Textqualifizierer für den Zellenwert vorhanden ist. Standard ist true.

```csharp
public bool HasTextQualifier { get; set; }
```

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasTextQualifierDemo
    {
        public static void Run()
        {
            // Erstelle CSV-Inhalt mit Textqualifizierern
            string csvContent = "\"Name\",\"Age\",\"City\"\n\"John\",30,\"New York\"\n\"Alice\",25,\"London\"";
            
            // Speichere CSV-Inhalt in einer temporären Datei
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvContent, Encoding.UTF8);

            // Erstelle TxtLoadOptions mit HasTextQualifier auf true gesetzt
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Lade die CSV-Datei mit Textqualifizierern
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Speichere die Arbeitsmappe, um das erfolgreiche Laden zu demonstrieren
            workbook.Save("Output.xlsx");

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


