---
title: "SaveOptions.ValidateMergedAreas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SaveOptions-Eigenschaft. Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden sollen"
type: docs
url: /de/net/aspose.cells/saveoptions/validatemergedareas/
---
## SaveOptions.ValidateMergedAreas property

Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.

```csharp
public bool ValidateMergedAreas { get; set; }
```

### Hinweise

Der Standardwert ist false.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyValidateMergedAreasDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Werte setzen und Zellen zusammenführen
            worksheet.Cells["A1"].PutValue("Merged Area");
            worksheet.Cells["A2"].PutValue("Test");
            worksheet.Cells.Merge(0, 0, 2, 1); // Merge A1:A2

            // Speicheroptionen erstellen, bei denen ValidateMergedAreas auf true gesetzt ist
            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                ValidateMergedAreas = true,
                MergeAreas = true
            };

            // Arbeitsmappe mit Validierung zusammengeführter Bereiche speichern
            workbook.Save("ValidateMergedAreasDemo.xlsb", saveOptions);

            Console.WriteLine("Workbook saved with merged areas validation.");
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


