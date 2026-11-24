---
title: "SaveOptions.SortNames"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SaveOptions-Eigenschaft. Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden"
type: docs
url: /de/net/aspose.cells/saveoptions/sortnames/
---
## SaveOptions.SortNames property

Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.

```csharp
public bool SortNames { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySortNamesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Workbook-Objekt
            Workbook workbook = new Workbook();
            
            // Fügen Sie Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Benannten Bereich erstellen
            worksheet.Cells.CreateRange("A2:B3").Name = "MyDataRange";

            // Speicheroptionen mit aktivierten SortNames erstellen
            XlsSaveOptions saveOptions = new XlsSaveOptions
            {
                SortNames = true
            };

            // Speichere die Arbeitsmappe
            workbook.Save("SortedNamesExample.xls", saveOptions);

            Console.WriteLine("Workbook saved with sorted named ranges.");
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


