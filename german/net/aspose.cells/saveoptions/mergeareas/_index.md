---
title: "SaveOptions.MergeAreas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SaveOptions-Eigenschaft. Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden sollen"
type: docs
url: /de/net/aspose.cells/saveoptions/mergeareas/
---
## SaveOptions.MergeAreas property

Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.

```csharp
public bool MergeAreas { get; set; }
```

### Hinweise

Der Standardwert ist false.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyMergeAreasDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten ausfüllen und zusammengeführte Zellen erstellen
            worksheet.Cells["A1"].PutValue("Merged Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Zellen A1:B1 zusammenführen
            worksheet.Cells.Merge(0, 0, 1, 2);

            // Speicheroptionen erstellen mit aktivierten MergeAreas
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MergeAreas = true;

            // Speichern mit Optimierung zusammengeführter Bereiche
            workbook.Save("MergeAreasDemo.xlsx", saveOptions);
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


