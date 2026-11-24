---
title: "PivotTable.EnableFieldDialog"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob das Dialogfeld für PivotTable-Felder verfügbar ist, wenn der Benutzer das PivotTable-Feld doppelklickt"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/enablefielddialog/
---
## PivotTable.EnableFieldDialog property

Gibt an, ob das Dialogfeld PivotTable‑Feld verfügbar ist, wenn der Benutzer das PivotTable‑Feld doppelt anklickt.

```csharp
public bool EnableFieldDialog { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableFieldDialogDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Demonstrieren Sie die EnableFieldDialog-Eigenschaft
            pivotTable.EnableFieldDialog = true;
            Console.WriteLine("EnableFieldDialog set to: " + pivotTable.EnableFieldDialog);

            // Ändern Sie die Eigenschaft und überprüfen Sie sie
            pivotTable.EnableFieldDialog = false;
            Console.WriteLine("EnableFieldDialog changed to: " + pivotTable.EnableFieldDialog);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTable_EnableFieldDialog_Example.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


