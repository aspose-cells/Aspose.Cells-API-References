---
title: "AutoFitterOptions.AutoFitMergedCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFitterOptions-Eigenschaft. Gibt an, ob die Zeilenhöhe automatisch angepasst wird, wenn Zellen in einer Zeile zusammengeführt werden. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/autofitteroptions/autofitmergedcells/
---
## AutoFitterOptions.AutoFitMergedCells property

Gibt an, ob die Zeilenhöhe automatisch angepasst wird, wenn Zellen in einer Zeile zusammengeführt werden. Der Standardwert ist false.

```csharp
[Obsolete("Use AutoFitterOptions.AutoFitMergedCellsType property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AutoFitMergedCells { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die AutoFitterOptions.AutoFitMergedCellsType-Eigenschaft. Diese Eigenschaft wird 12 Monate nach Dezember 2018 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten erstellen und Zellen zusammenführen
            worksheet.Cells["A1"].PutValue("This is a test of AutoFitMergedCells property");
            worksheet.Cells.Merge(0, 0, 3, 3); // Merge cells A1:C3

            // AutoFitterOptions erstellen und AutoFitMergedCells festlegen
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;

            // Zeilen mit zusammengeführten Zellen automatisch anpassen
            worksheet.AutoFitRows(options);

            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitMergedCellsExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


