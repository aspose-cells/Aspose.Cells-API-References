---
title: "WorksheetCollection.ActiveSheetIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Gibt den Index des aktiven Arbeitsblatts an, wenn die Tabelle geöffnet wird"
type: docs
url: /de/net/aspose.cells/worksheetcollection/activesheetindex/
---
## WorksheetCollection.ActiveSheetIndex property

Stellt den Index des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird.

```csharp
public int ActiveSheetIndex { get; set; }
```

### Hinweise

Der Blattindex ist nullbasiert.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetIndexDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe mit 3 Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Setzen Sie den Index des aktiven Blatts auf 1 (zweites Blatt)
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Überprüfen Sie das aktive Blatt
            Console.WriteLine("Active Sheet: " + workbook.Worksheets[workbook.Worksheets.ActiveSheetIndex].Name);

            // Speichere die Arbeitsmappe
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ActiveSheetDemo.xlsx");
            workbook.Save(outputPath);

            Console.WriteLine("File saved to: " + outputPath);
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


